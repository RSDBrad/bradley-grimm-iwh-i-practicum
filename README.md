# Welcome to the Integrating With HubSpot I: Foundations Practicum

This repository is for the Integrating With HubSpot I: Foundations course. This practicum is one of two requirements for receiving your Integrating With HubSpot I: Foundations certification. You must also take the exam and receive a passing grade (at least 75%).

To read the full directions, please go to the [practicum instructions](https://app.hubspot.com/academy/l/tracks/1092124/1093824/5493?language=en).

**Put your HubSpot developer test account custom objects URL link here:** https://app-na3.hubspot.com/contacts/343654883/objects/2-250710885/views/all/list

## About this project

This Node.js app uses Express, Axios, and Pug to display Pet
records from HubSpot and create new records through a form.

The Pet properties are name, species, and bio.

## HubSpot test account

https://app-na3.hubspot.com/contacts/343654883/objects/2-250710885/views/all/list

## Local setup

1. Install Node.js LTS.
2. Clone this repository.
3. Run `npm install`.
4. Create a `.env` file in the project root with these settings:

   PRIVATE_APP_ACCESS_TOKEN=your-private-app-token
   CUSTOM_OBJECT_ID=2-250710885
   PORT=3000

5. Run `node index.js`.
6. Open http://localhost:3000.

The private app needs read and write access for:
- crm.schemas.custom
- crm.objects.custom
- crm.objects.contacts

The `.env` file is excluded from Git. Never commit an access token.

## Routes

- GET / — displays Pet records in a table.
- GET /update-cobj — displays the creation form.
- POST /update-cobj — creates a Pet and redirects to the homepage.

## Testing completed

- Confirmed existing Pets display with Name, Species, and Bio.
- Created Buddy through the form.
- Confirmed the redirect and Buddy's appearance in the table.

___
## Tips:
- Commit to your repository often. Even if you make small tweaks to your code, it’s best to be committing to your repository frequently.
- The subject of the custom object is up to you. Feel free to get creative!
- Please create a test account and include your private app access token in your repo.
- Ensure you re-merge any working branches into the main branch.
- DO NOT ADD YOUR PRIVATE APP TOKEN TO YOUR REPOSITORY. 

## Pre-requisites:
- Using [Node](https://nodejs.org/en/download) and node packages
- Using [Express](https://expressjs.com/en/starter/installing.html)
- Using [Axios](https://axios-http.com/docs/intro)
- Using [Pug templating system](https://pugjs.org/api/getting-started.html)
- Using the command line
- Using [Git and GitHub](https://product.hubspot.com/blog/git-and-github-tutorial-for-beginners)

## Requirements
- All work must be your own. During the grading process we will check the revision history. Submissions that do not meet this requirement will not be considered.
- You must have at least two new routes in your index.js file and one new pug template for the homepage.
- You must create a developer test account and link to it in your README.md file. Submissions that do not meet this requirement will not be considered.
