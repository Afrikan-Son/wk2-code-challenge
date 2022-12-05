# JavaScript Week 2 Code Challenge

# Learning Goals

Implementing a mini web app to practice on array iteration, DOM, Events, and Server communications.

# Description

For this challenge, you will be working on Flataculties, an app where you can vote for the cutest animal! You will use a local API and build out the frontend for our app, Flatacuties.

The instructions below will walk you through the process of ideation and planning your app: deciding on your user interface, planning how the information will be laid out on the page, etc.

# Project Setup & Pre-requisite Data

1. In your project directory, create a db.json file and use this data (https://docs.google.com/document/d/1EUcHU9gkydR3IfJDTebW5iNHP2BCMRcv508R7BAXSvo/edit) as it links to an external site for your server DB.
2. Run this command to get the backend started: 'json-server --watch db.json'
3. Test your server by visiting this route in the browser: http://localhost:3000/characters

## Getting Started

Make sure to have th following on your computer:
1. A computer that runs on either of the following; (Windows 7+, Linux, Mac OS)
2. Nodejs 9.0

# Install requirements

Clone the repository to your computer and `npm install` in the repo folder after cloning in terminal.

## Setup

Run this command to get the backend started:

```sh
json-server --watch db.json
```
Test your server by visiting this route in the browser:

[http://localhost:3000/characters](http://localhost:3000/characters)

Then, open the `index.html` file on your browser to run the application.

Write your code in the `src/index.js` file. The base URL for your API will be
[http://localhost:3000](http://localhost:3000).

## Deliverables

As a user, I can:

1. See all characters names in a `div` with the id of `"character-bar"`. Create
   a `span` tag with the character's name and add it the `div#character-bar`
   once you have retrieved the character data from the server. You will need to
   make a GET request to the following endpoint to retrieve the character data:

   ```txt
   GET /characters

   Example Response:
   [
    {
      "id": 1,
      "name": "Mr. Cute",
      "image": "https://thumbs.gfycat.com/EquatorialIckyCat-max-1mb.gif",
      "votes": 0
    },
    {
      "id": 2,
      "name": "Mr. Monkey",
      "image": "https://thumbs.gfycat.com/FatalInnocentAmericanshorthair-max-1mb.gif",
      "votes": 0
    },
    ...
   ]
   ```

2. When the character in the `div#character-bar` is clicked, display the
   character's details in the `div#detailed-info`. You can either use the
   character information from your first request, or make a new request to this
   endpoint to get the character's details:

   ```txt
   GET /characters/:id

   Example Response:
   {
    "id": 1,
    "name": "Mr. Cute",
    "image": "https://thumbs.gfycat.com/EquatorialIckyCat-max-1mb.gif",
    "votes": 0
   }
   ```

3. When the `form#votes-form` is submitted, add the number of votes from
   the input field to the character displayed in the `div#detailed-info`. **No
   persistence is needed**.


# Authors
This project was contributed to by:
- [Mark Wanjau](https://github.com/Afrikan-Son)

# License
The project is licensed under ISC.