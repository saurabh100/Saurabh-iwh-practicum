# Integrating With HubSpot I: Foundations Practicum

This repository contains my project for the HubSpot Academy **Integrating With HubSpot I: Foundations Practicum**.

## Project Overview

I built a Node.js application that connects with HubSpot CRM using the HubSpot API.

For this project, I created a custom CRM object called **Video Game** with three properties:

- Name
- Publisher
- Price

The application retrieves Video Game records from HubSpot and displays them in a table. It also provides a form to create new Video Game records directly in HubSpot.

## HubSpot Custom Object

**Custom Object:** Video Game

**Custom Object Type ID:** `2-70227904`

**HubSpot Custom Object URL:**

https://app.hubspot.com/contacts/52112263/objects/2-70227904/views/all/list

## Application Routes

### `GET /`

Fetches Video Game records from HubSpot and displays them in a table.

### `GET /update-cobj`

Displays the form for adding a new Video Game record.

### `POST /update-cobj`

Creates a new Video Game record in HubSpot using the CRM API and redirects back to the homepage.

## Technologies Used

- Node.js
- Express
- Axios
- Pug
- HubSpot CRM API
- Git
- GitHub

## Project Structure

```text
.
├── public/
│   └── css/
│       └── style.css
├── views/
│   ├── index.pug
│   └── update-cobj.pug
├── .gitignore
├── index.js
├── package.json
└── README.md

Running the Application

Install the dependencies:

npm install

Create a .env file in the project root:

PRIVATE_APP_ACCESS=YOUR_HUBSPOT_PRIVATE_APP_ACCESS_TOKEN

Start the application:

node index.js

The application will be available at:

http://localhost:3000
Security

The HubSpot private app access token is stored in the .env file and is not included in this repository.

The .env file is excluded using .gitignore.

Practicum

This project was created as part of the Integrating With HubSpot I: Foundations practicum and demonstrates working with HubSpot custom objects, CRM APIs, Express routes, Axios requests, and Pug templates.