# Server installation guide


## ES2

TODO: What instance, how it was configured?

Add additional swap memory

```
sudo fallocate -l 2G /swapfile  
sudo chmod 600 /swapfile  
sudo mkswap /swapfile  
sudo swapon /swapfile  
sudo swapon -show  
echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab
```

### Access

Provide us with your public key and `ssh ubuntu@13.53.140.53` into the server.
If you are a teacher, your key should already be added.

### Docker & docker-compose

TODO: How were they installed?

`docker-compose.frontend.yml`, `docker-compose.backend.yml` and `.env` files are deployed to the server by gitlab pipeline
and are subsequently used to configure, run and update our services.

### Gitlab runner

TODO: How was the gitlab-runner itself installed?

Gitlab runner instance is configured using the following `/etc/gitlab-runner/config.toml` file:

* token omitted, obtain one from [runners settings](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/settings/ci_cd#js-runners-settings)

```
concurrent = 2
check_interval = 0

[session_server]
  session_timeout = 1800

[[runners]]
  name = "spacevolcanoes-runner"
  url = "https://gitlab.cs.ttu.ee/"
  token = "token-omitted"
  executor = "docker"
  [runners.custom_build_dir]
  [runners.cache]
    [runners.cache.s3]
    [runners.cache.gcs]
    [runners.cache.azure]
  [runners.docker]
    tls_verify = false
    image = "docker:19.03.8"
    privileged = true
    disable_entrypoint_overwrite = false
    oom_kill_disable = false
    disable_cache = false
    volumes = ["/cache"]
    shm_size = 0
    limit = 1
```

### Gitlab pipeline

Deploy to our production server uses the following 
[Gitlab environment variables](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/settings/ci_cd#js-cicd-variables-settings):

- `SSH_PRIVATE_KEY` - to log in to the production server 
- `DOCKER_USER` and `DOCKER_PASS` - to push the built docker images to Docker Hub
- `DOCKER_SECRETS` to populate the `.env` file on the server which passes on variables to services via docker-compose
