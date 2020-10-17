# Business analysis overview

A receipt analysis service which will provide an overview and help with the classification of the purchased entries.

# User stories

🔥 Must have

🎁 Nice to have

⚗️ Negotiable

## Unauthorized visitor

- [X] 🔥**AS A** visitor
  **I WANT** to see some statistics and examples
  **SO THAT** I would have confidence in using the service.
  [☁#24](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/24)
  [🖥#11](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/11)

- [ ] 🎁**AS A** visitor
  **I WANT** to see terms of service before signing up
  **SO THAT** I would know what I am getting myself into.

- [ ] 🔥**AS A** visitor
  **I WANT** the website look attractive and easily usable
  **SO THAT** I would trust the service and be more likely to start using it.
  [🖥#9](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/9)

- [ ] 🔥**AS A** visitor
  **I WANT** to create an account with the service
  **SO THAT** my data would remain connected to me.
  [☁#9](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/9)
  [🖥#8](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/8)

## Registered customer

- [X] 🔥**AS A** customer
  **I WANT** to upload an image of my receipt
  **SO THAT** I could get the entries on it back in text form.
  [🖥#1](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/1)

- [ ] 🎁**AS A** customer
  **I WANT** to crop my image in the upload form
  **SO THAT** the most relevant part (the receipt) and less of the background gets stored on the service.
  [🖥#2](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/2)

- [X] 🔥**AS A** customer
  **I WANT** to provide fixes and feedback for the text entries
  **SO THAT** my data would be identified and classified correctly.
  [🖥#3](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/3)
  [☁#5](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/5)

- [X] 🔥**AS A** customer
  **I WANT** my uploaded image and entry data to be saved
  **SO THAT** I wouldn't need to upload them multiple times.
  [☁#2](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/2)
  [☁#3](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/3)

- [X] 🔥**AS A** customer
  **I WANT** to see an overview list of my previously saved receipts together with a summary
  **SO THAT** I would know which receipts I've already uploaded to the service.
  [🖥#4](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/4)
  [☁#6](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/6)

- [ ] ⚗️**AS A** customer
  **I WANT** to sort and filter the receipts list by date/shop/sum
  **SO THAT** I could get a better overview about my expenses.

- [X] 🔥**AS A** customer
  **I WANT** to be able to open up and see a detailed receipt page
  **SO THAT** I could see which entries were covered by this receipt.
  [🖥#5](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/5)
  [☁#7](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/7)

- [ ] ⚗️**AS A** customer
  **I WANT** to be able to view a summary list of entries gathered from my receipts
  **SO THAT** I could get an overview of my purchases.

- [ ] 🎁**AS A** customer
  **I WANT** to be able to sort and filter the individual entries
  **SO THAT** I could get a better insight into my shopping behavior.

- [ ] 🔥**AS A** customer
  **I WANT** to be able to open up and see a detailed entry page
  **SO THAT** I could see how many times, for which prices and where I have purchased this entry.
  [☁#10](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/10)
  [🖥#7](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/7)

- [ ] 🔥**AS A** customer
  **I WANT** to be able to delete my receipts and entries tied to them
  **SO THAT** I could avoid accidental duplicates and protect my privacy.
  [☁#8](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/8)
  [🖥#6](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/issues/6)

- [ ] 🎁**AS A** customer
  **I WANT** to be able to delete my account
  **SO THAT** I could protect my privacy.

- [ ] 🎁**AS A** customer
  **I WANT** the service to provide the entries from my receipt image as text
  **SO THAT** I wouldn't have to insert that manually.
  [☁#8](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/issues/12)

- [ ] 🎁**AS A** customer
  **I WANT** the service to attempt to categorize the entries from my receipts
  **SO THAT** I wouldn't have to insert that manually.

- [ ] 🎁**AS A** customer
  **I WANT** the service to provide the metadata (store/date/time/location) from my receipt image as text 
  **SO THAT** I wouldn't have to insert that manually.

- [ ] 🎁**AS A** customer
  **I WANT** to be able to edit the metadata (email mostly) related to my account
  **SO THAT** I wouldn't have to make a new account, if said metadata changes.
