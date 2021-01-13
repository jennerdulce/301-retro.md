# 301-retro.md

## Retro 1: and Responsive Web Design
### 1. What went well, that I might forget if I don’t write down?
```
@media (max-width: #){
    //code
}
```
- make line height the same as the height of the container to align vertically.  Only works with 1 line of text
- mobile first design
- box-sizing: border-box *** adds a border and keeps set width

### 2. What did I learn today?
- box-sizing is very helpful.

### 3. What should I do differently next time?
- start with mobile

### 4. What still puzzles me, or what do I need to learn more about?
- How padding and text content will effect the sizing and dimensions of everything.


## Retro 2: jQuery, Events, and The DOM
### 1. What went well, that I might forget if I don’t write down?
- A-synchronization: other code will continue to run while the .ajax method retrieves the JSON data. Trying to render/work with data at this point may be undefined because the render methods are trying to work with data that has not finished processing yet
- When cloning a template, use .find('element within template') to target the elements in the clone.
  - i.e $template.find('h2') or $template.find('p')
- When dealing with a dropdown or 'select' element. use on'change' as the event handler. Instead of on'click' for the options.

### 2. What did I learn today?
- I learned how to use $.ajax to retrieve data from a JSON file. using a .then() method to work with each individual object within that file and extract the information.
- There is no shame in asking for help!

### 3. What should I do differently next time?
- Nothing in particular. Make sure you read the assignment thoroughly 

### 4. What still puzzles me, or what do I need to learn more about?
- I need to confidently be able to type:
- ajax/then methods
- arrow function
- forEach functions

## Retro 3: Flexbox and Templating
### 1. What went well, that I might forget if I don’t write down?
- Mustache {{ }}
- STEPS:
1. Add CDN
2. Create Script with id="unique template name" type="x-tmpl-mustache"
3. Make variable and target the template (which is a script)
4. Make a variable and run the Mustache.render(insert template, { add keys and values for template }
5. Append to where you want the script to be displayed
- Setting a variable to the value of a button selected on event listeners
- Adding multiple classes on an element
- Hiding/showing what you want based on .hide() and .show() classes
- .empty() and rerender
- Sort Functions
- you can a return statement at the beginning instead of at the end

### 2. What did I learn today?
- Mustache
- Flexbox
- Sorting objects

### 3. What should I do differently next time?
- Take one step at a time and know your code so you know where to look and how to fix problems

### 4. What still puzzles me, or what do I need to learn more about?
- How to make all sorting options work with each other


## Retro 4: Responsive Web Design and RegEx
### 1. What went well, that I might forget if I don’t write down?
- When using Grid or Flexbox. You do not need to set any widths or heights.
- Make sure that boxes or elements you want to align are directly a child of a parent container that has been set to display: grid/flexbox
- When using a forEach for REGEX. matching returns an ARRAY with a single value in it (the cities problem). When you retrieve the information, you have to access it by the index at [0].
    - Note: There will only be 1 item in the array so thats why you always have to access the value at 0

### 2. What did I learn today?
- Grid is great. I used grid-template-area and worked like magic.
- Regex is confusing

### 3. What should I do differently next time?
- I tried to refactor the code I previously had. It was better to just completely start over

### 4. What still puzzles me, or what do I need to learn more about?
- REGEX: Remember to use if statements
- Remember that you can create more than 1 regex criteria and use both to filter out data that you want.


## Retro 5: Heroku Deployment
### 1. What went well, that I might forget if I don’t write down?
- .slice()
- .split()
-.join()

### 2. What did I learn today?
- That CSS can get very messy if you do not separate code into mutiple CSS files.

### 3. What should I do differently next time?
- Alter 1 thing at a time
- Make sure that I keep chunks of code together so that it is more organized

### 4. What still puzzles me, or what do I need to learn more about?
- How to build a server and what each line means when building it.


## Retro 6: NODE, EXPRESS, and APIs
### 1. What went well, that I might forget if I don’t write down?
- How to build a server. However, this skill will continue to be developed for the rest of the cirriculum

### 2. What did I learn today?
- I learned that we are able to access input through AJAX SETTINGS that is in the app.js file in the front it. Data must be in AJAX settings in order to be retrieved in the backend.

### 3.What should I do differently next time?
- Nothing I feel I should do differently next time. Had a good understanding and the lab went smoothly

### 4.What still puzzles me, or what do I need to learn more about?
- Exactly what each part does. We learned specific commands but would like a more in-depth explanation as to how things work. Or is it just better to accept the backend magic?


## Retro 7: APIs
### 1. What went well, that I might forget if I don’t write down?
- Things you need to use an API:
    1. within handler that you want
    2. create key variable with process.env.KEYNAME
    3. create a url variable with API URL and insert keyname and other url parameters you may need
    4. import superagent and request using `superagent.get(url)`
- how to use REGEX:
    1. create regex variable: `let regex = / /g
    2. create string (if needed)
    3. use `regex.test(string)` or `string.match(regex)`

### 2. What did I learn today?
- superagent is used to talk to APIs
    - request data and in hopes to receive a promise
    - we BUILD the requet within the `.then()` method within the superagent request
- use `.filter()` to filter out the items/objects you need within a big database
    - USE REGEX
    - filter only returns whole items
    - cannot choose what you want within an item/object
    - uses BOOLEAN STATEMENTS whether to add the current value to the array
- use `.map()` to retrieve the specific information that you want from the filter array that was created by `.filter()`.

### 3.What should I do differently next time?
- Review notes more often

### 4.What still puzzles me, or what do I need to learn more about?
- I need to study terminology to better understand/explain efficiently which will come in due time


## Retro 8: SQL & Databases
### 1. What went well, that I might forget if I don’t write down?
- How to talk to databases
    1. create a database
        - `psql`
        - `CREATE DATABASE database_name`
    2. create `client` variable
        - `const client = new pg.Client(process.env.DATABASE_URL)`
    3. add .env file with a DATABASE_URL
        - `DATABASE_URL = postgres://localhost5432/database_name`
    4. create a schema.sql file
        - this file creates a table within the database you connect to
        ```
        DROP TABLE IF EXISTS table_name
        
        CREATE TABLE table_name (
            column1 datatype,
            column1 datatype,
            column1 datatype,
            column1 datatype,
        );
        ```
      
    5. connect server to database
        - psql -f schema.sql -d database_name
        - will create the table
    6. in server.js
        - `client.on('error', err () => {throw err;})`
        - ```client.connect()
            .then( () => {
                app.listen(PORT, () => {
                    console.log(PORT)
                    console.log(client.connectionParameters.database)```
    7. PARTS TO MAKE A REQUEST TO THE DATABASE
        - SQL variable: should contain a SQL statement
        - safeValues variable: should contain values you want to insert into the SQL statement
        - client.query(SQL, safeValues)
           
### 2. What did I learn today?
- We want to add to the database during the API call.
    - This makes sense because we already have the information from the promise, so we use that information to store the data and also repsond at the moment
    - the next time we query for something, we will first go through the database, if it exists, it will pull the information from the database, if not, then the api call will run adding the information.
 
 - you can use different values for .filter().
    - you can set it to [], {}, 0, '',

### 3.What should I do differently next time?
- nothing, i am please with the results and growth this past week.

### 4.What still puzzles me, or what do I need to learn more about?
- starting to get a hang of the web request response cycle! all making sense.


## Retro 9: Refactoring and SQL
### 1. What went well, that I might forget if I don’t write down?
- Refactoring is farily simple.
- Sometimes API urls won't allow you to set query parameters in the URL or API Key.. 
- use a `.set()` to set API Key as a header 
- use `.query(queryList)` to attach the queryList

### 2. What did I learn today?
- I learned how to impletment headers and queryLists to API requests using `.set()` and `.query()`
- ALL APIs work differently, however reading the docs will give you the solution you need

### 3. What should I do differently next time?
- Nothing in mind, Need to keep pushing and maybe push a little harder.

### 4. What still puzzles me, or what do I need to learn more about?
- How the front-end makes the requests to the back end and how the front end sends data (an object which was passed to the front end) to the backend for further usage

