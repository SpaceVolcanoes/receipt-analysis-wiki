# Receipt analysis service
![g272](/g272.png)

We are building a automatic shopping receipt data capture and analysis service where users can upload a picture of their latest receipts and get a detailed overview of their spending habits and trends to help them manage their money easier. 

**In part 1 we will accomplish the following:**
- [x] Have a basic backend REST API that allows us to upload images 
- [x] Backend that stores receipt information to database
- [x] Have a Vue frontend that connects to our backend
- [x] Have a detailed receipt page that displays the enries covered by a receipt

**In part 2 we will accomplish the following:**
- [ ] AWS server setup where our backend docker container runs and frontend is delivered
- [ ] Automatic deploy to our server
- [ ] Automatically run tests in our pipeline

**By the end of part 3 we will have:**
- [ ] A working website online that is able to produce receipt data from (some) images
- [ ] User account login page so that the data will remain connected with the customer
- [ ] Provide some statistics/insight for our users about their shopping behavior
---
- [Business analysis](/page/business_analysis)
- [How are we making money?](/page/money)

## The Team
- **Team Lead and Project Manager**:  Jaak Kütt  @jakutt
- **Lead Backend Developer**:  Kristjan Kõiv  @krikoi
- **Lead Frontend Developer**:  Kristajn Koitla  @krkoit
- **DevOps Engineer**:  Mart Kaasik  @markaa

## Retros

- [Spawn point](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/wikis/Spawn-point-retro) - milestone [front](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/milestones/1) / [back](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/milestones/1)
- [Dumpster Fire](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/wikis/Dumpster-Fire-retro) - milestone [front](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-frontend/-/milestones/2) / [back](https://gitlab.cs.ttu.ee/jakutt/team-02-spacevolcanoes-backend/-/milestones/2)

## Supporting materials

- Template for creating new issues: [Issue template](Issue-template)
- Task description [ITI0203 Project](https://olegpahhomov.gitlab.io/iti0203-2020/iti0203-2020-project/)
- Blog post about [OCR](https://nanonets.com/blog/receipt-ocr/)
- Examples about [tesseract usage](https://stackoverflow.com/questions/37745519/use-pytesseract-ocr-to-recognize-text-from-an-image)
- Example for cleaning background part from the image with [PixelLib](https://towardsdatascience.com/change-the-background-of-any-image-with-5-lines-of-code-23a0ef10ce9a)
