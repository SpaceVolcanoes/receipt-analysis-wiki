# Features

Our features described as user stories together with links to implementation tickets. Roles mentioned in the stories:

- visitor, unauthorized page visitor (Guest)
- customer, registered and logged-in customer (User)
- administrator, logged-in user with all privileges (Admin)

# Current scope (8)

- [X] **AS A** visitor
  **I WANT** to see some statistics and examples
  **SO THAT** I would have confidence in using the service.

  **Issues:**
  [☁#24](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/24)
  [🖥#11](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/11)

- [X] **AS A** customer
  **I WANT** to crop my image in the upload form
  **SO THAT** the most relevant part (the receipt) and less of the background gets stored on the service.

  **Issues:**
  [🖥#2](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/2)

- [X] **AS A** customer
  **I WANT** my uploaded image and entry data to be saved
  **SO THAT** I wouldn't need to upload them multiple times.

  **Issues:**
  [🖥#1](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/1)
  [☁#2](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/2)
  [☁#3](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/3)

- [X] **AS A** customer
  **I WANT** to provide fixes and feedback for the text entries
  **SO THAT** my data would be identified and classified correctly.

  **Issues:**
  [🖥#3](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/3)
  [☁#5](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/5)

- [X] **AS A** customer
  **I WANT** to see an overview list of my previously saved receipts together with a summary
  **SO THAT** I would know which receipts I've already uploaded to the service.

  **Issues:**
  [🖥#4](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/4)
  [☁#6](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/6)

- [X] **AS A** customer
  **I WANT** to be able to open up and see a detailed receipt page
  **SO THAT** I could see which entries were covered by this receipt.

  **Issues:**
  [🖥#5](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/5)
  [☁#7](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/7)

- [X] **AS A** customer
  **I WANT** to be able to delete my receipts and entries tied to them
  **SO THAT** I could avoid accidental duplicates and protect my privacy.

  **Issues:**
  [☁#8](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/8)
  [🖥#6](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/6)

- [X] **AS AN** administrator
  **I WANT** to be able to see and delete images customers have uploaded
  **SO THAT** I could police compliance to our terms of service.

  **Issues:**
  [☁#47](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/47)
  [🖥#19](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/19)

# Future plans (12)

- [ ] **AS A** visitor
  **I WANT** to see terms of service before signing up
  **SO THAT** I would know what I am getting myself into.

  **Estimated:**
  Time: 2h,
  Complexity: 1

- [ ] **AS A** visitor
  **I WANT** the website look attractive and easily usable
  **SO THAT** I would trust the service and be more likely to start using it.

  **Issues:**
  [🖥#9](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/9)

  **Estimated:**
  Time: 4h,
  Complexity: 2

- [ ] ️**AS A** customer
  **I WANT** to sort and filter the receipts list by date/shop/sum
  **SO THAT** I could get a better overview about my expenses.

  **Estimated:**
  Time: 5h,
  Complexity: 3

- [ ] ️**AS A** customer
  **I WANT** to be able to view a summary list of entries gathered from my receipts
  **SO THAT** I could get an overview of my purchases.

  **Estimated:**
  Time: 6h,
  Complexity: 3

- [ ] **AS A** customer
  **I WANT** to be able to sort and filter the individual entries
  **SO THAT** I could get a better insight into my shopping behavior.

  **Estimated:**
  Time: 8h,
  Complexity: 5

- [ ] **AS A** customer
  **I WANT** to be able to open up and see a detailed entry page
  **SO THAT** I could see how many times, for which prices and where I have purchased this entry.

  **Issues:**
  [☁#10](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/10)
  [🖥#7](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/7)

  **Estimated:**
  Time: 7h,
  Complexity: 5

- [ ] 🎁**AS A** customer
  **I WANT** the service to provide the entries from my receipt image as text
  **SO THAT** I wouldn't have to insert that manually.

  **Issues:**
  [☁#12](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/12)
  [☁#13](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/13)

  **Estimated:**
  Time: 11h,
  Complexity: 13

- [ ] **AS A** customer
  **I WANT** to be able to delete my account
  **SO THAT** I could protect my privacy.

  **Estimated:**
  Time: 2h,
  Complexity: 2

- [ ] **AS A** customer
  **I WANT** the service to attempt to categorize the entries from my receipts
  **SO THAT** I wouldn't have to insert categories manually.

  **Estimated:**
  Time: 16h,
  Complexity: 20

- [ ] **AS A** customer
  **I WANT** the service to provide the metadata (store/date/time/location) from my receipt image as text
  **SO THAT** I wouldn't have to insert that manually.

  **Estimated:**
  Time: 16h,
  Complexity: 20

- [ ] **AS A** customer
  **I WANT** to be able to edit the metadata (email mostly) related to my account
  **SO THAT** I wouldn't have to make a new account, if said metadata changes.

  **Estimated:**
  Time: 4h,
  Complexity: 3

# Not for grading / auth related (1)

- [X] **AS A** visitor
  **I WANT** to create an account with the service
  **SO THAT** my data would remain connected to me.

  **Issues:**
  [☁#9](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/9)
  [🖥#8](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/8)
