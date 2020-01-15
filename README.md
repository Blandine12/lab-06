# lab-06

Author: Blandine Dasilveira

Version: 1.0.0 (increment the patch/fix version number if you make more commits past your first submission)

 Overview
The city explorer projet is a project for the Back end to give data to the front End, and that will allow user to request weather

## Getting Started
<!-- What are the steps that a user must take in order to build this app on their own machine and get it running? -->

Architecture
BACK End will utilizes JavaScript and some libraries
- Node.js
- Express.js
- Dotenv
- Cors

Change Log

01-04-2020 12:59pm - Application now has a fully-functional express server, with a GET route for the location resource.

## Credits and Collaborations
<!-- Give credit (and a link) to other people or resources that helped you build this application. -->


- SET UP REPO:
.env - with your PORT. Make sure this file is in your .gitignore.
README.md - with documentation regarding your lab and its current state of development. Check the "documentation" section below for more details on how that should look AT MINIMUM
.gitignore - with standard NodeJS configurations
.eslintrc.json - with Code 301 course standards for the linter
package.json - with all dependencies and any associated details related to configuration. The dependencies needed for today's lab include: express, dotenv, and cors.
Note that the package-lock.json file is automatically created when dependencies are installed and ensures that future installations of the project use the same versions of the dependencies.
data directory - containing geo.json and darksky.json
Deploy your basic express server to Heroku.

Number and name of feature: Feature 1

Estimate of time needed to complete: 20 mn

Start time: 09:30

Finish time: 09:50

Actual time needed to complete: 

- FEATURE 2:

Given that a user enters a valid location in the input

When the user clicks the "Explore!" button

Then the map will be populated with the location centered on the latitude and longitude of the search query

Endpoint:
/location

Example Response:

{
  "search_query": "seattle",
  "formatted_query": "Seattle, WA, USA",
  "latitude": "47.606210",
  "longitude": "-122.332071"
}
Features
Delete
0%
Create a route with a method of get and a path of /location. The route callback should invoke a function to convert the search query to a latitude and longitude. The function should use the provided JSON data.
A constructor function will ensure that each object is created according to the same format when your server receives the external data. Ensure your code base uses a constructor function for this resource.
Return an object which contains the necessary information for correct client rendering. See the sample response.
Deploy your updated express server to Heroku.
Confirm that your route is responding as expected by entering your deployed backend URL on the City Explorer app's welcome page. Then search for a location. You should see the map, but not any other data yet.

Number and name of feature: Feature 2

Estimate of time needed to complete: 1 hour

Start time: 09:50

Finish time: 11:59

Actual time needed to complete: 

- FEATURE 3

Given that a user enters a valid location in the input

When the user clicks the "Explore!" button

Then the weather forecast for the upcoming eight days will be displayed in the browser

Endpoint:
/weather

Example Response:

[
  {
    "forecast": "Partly cloudy until afternoon.",
    "time": "Mon Jan 01 2001"
  },
  {
    "forecast": "Mostly cloudy in the morning.",
    "time": "Tue Jan 02 2001"
  },
  ...
]
Features
Delete
0%
Create a route with a method of get and a path of /weather. The callback should use the provided JSON data.
A constructor function will ensure that each object is created according to the same format when the server receives data. Ensure your code base uses a constructor function for this resource.
Confirm that your route is responding as expected by entering your deployed backend URL on the City Explorer app's welcome page. Then search for a location. You should see the map, and now weather data.
Using each weather object of the result, return an array of objects for each day of the response which contains the necessary information for correct client rendering. See the sample response.
Deploy your updated server code to Heroku.

Number and name of feature: Feature 3

Estimate of time needed to complete: 

Start time: 

Finish time: 

Actual time needed to complete: 


- FEATURE 4

Given that a user does not enter a valid location in the input

When the user clicks the "Explore!" button

Then the user will receive an error message on the page and the data will not be rendered properly

Endpoints:
/location, /weather

Example Response:

{
  status: 500,
  responseText: "Sorry, something went wrong",
  ...
}
Features
Delete
0%
Confirm that your route is responding as expected by entering your deployed backend URL on the City Explorer app's welcome page. Then search for an invalid location. The network inspector panel should show a 500 for the response to the AJAX query.
Create a function to handle errors from any API call.
Send a status of 500 and an error message to the client.
Deploy your updated sever code to Heroku.



Number and name of feature: Feature 4

Estimate of time needed to complete: 

Start time: 

Finish time: 

Actual time needed to complete: 

