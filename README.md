# QA-Tests-of-back-and-front-end
On this repository we will be testing the backend ok and API Rest and also testing the front end with cypress and NodeJs.

# Setups for your project
You'll need to install NodeJs, install cypress in your project folder with, and then run cypress.

# pluggins for cypress - xpath
¿How can I integrate the xpath method of selenium on cypress?
R= very simple, install on your proyect npm install cypress-path, then configure in your index.js file as require('cypress-xpath')

and in your test use it like cy.xpath('xpath build by yourself')

# To test Back End : file path: integration/examples/example.js

We'll be using axios, to make call the API. Cypress has also its methods, but it gets tricky somethimes with asyncronization.
First: search with the following url https://api.openbrewerydb.org/breweries/autocomplete?query="lagunitas"
Second: Search all the records who's name is "lagunitas brewing co"
thrid: search in the results of the previous search, the Id's who's contains "state" = "california" in their details
finally: assert if the element id is 761, name is "lagunitas brewing co", street "1280 n mcdowell blvd", and phone 7077694495

# to test Front End: file path: integration/examples/example.js

To test the front end

1. Get to https://www.fravega.com
2. Search heladeras
3. Filter for samsung brand

a) Assert that the number of results match with what we are seeing
b) Verify wich of those post has samsung as title 
c) Verify that in the breadcrumbers we have "heladeras con freezer"
