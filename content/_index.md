# Receipt analysis service
![g272](/g272.png)

We are building an automatic shopping receipt data capture and analysis service where users can upload a picture of their latest receipts and get a detailed overview of their spending habits and trends to help them manage their money easier. 

Visit our website at [receipt.modalstudio.com](https://receipt.modalstudio.com/).

See service [status](https://stats.uptimerobot.com/qDK0gIO086).

## Development story

**Part 3:**
- [X] Users can register and login so that their data remains more private and connected to themselves
- [X] A working website online that is able to produce receipt data from (some) images

**Part 2:**
- [x] AWS server setup where our backend docker container runs and frontend is delivered
- [x] Automatic deploy to our server
- [x] Automatically run tests in our pipeline

**Part 1:**
- [x] Have a basic backend REST API that allows us to upload images 
- [x] Backend that stores receipt information to database
- [x] Have a Vue frontend that connects to our backend
- [x] Have a detailed receipt page that displays the enries covered by a receipt

## The Team
- **Team Lead and Project Manager**:  Jaak Kütt  @jakutt
- **Lead Backend Developer**:  Kristjan Kõiv  @krikoi
- **Lead Frontend Developer**:  Kristjan Koitla  @krkoit
- **DevOps Engineer**:  Mart Kaasik  @markaa

## Repositories

- [Frontend](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/)
- [Backend](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/)

## Retros

- [Spawn point](/page/retro-spawn-point) - milestone [front](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/milestones/1) / [back](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/milestones/1)
- [Dumpster Fire](/page/retro-dumpster-fire) - milestone [front](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/milestones/2) / [back](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/milestones/2)
- [Mild food poisoning](/page/retro-mild-food-poisoning) - milestone [front](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/milestones/3) / [back](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/milestones/3)
- [Abandoned cabin](/page/retro-abandoned-cabin) - milestone [front](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/milestones/4) / [back](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/milestones/4)
- [Frozen lake](/page/retro-frozen-lake) - milestone [front](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/milestones/5) / [back](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/milestones/5)

## Supporting materials

- Template for creating new issues: [Issue template](Issue-template)
- Task description [ITI0203 Project](https://olegpahhomov.gitlab.io/iti0203-2020/iti0203-2020-project/)
- Blog post about [OCR](https://nanonets.com/blog/receipt-ocr/)
- Examples about [tesseract usage](https://stackoverflow.com/questions/37745519/use-pytesseract-ocr-to-recognize-text-from-an-image)
- Example for cleaning background part from the image with [PixelLib](https://towardsdatascience.com/change-the-background-of-any-image-with-5-lines-of-code-23a0ef10ce9a)
