# 301-retro.md

## SMACSS and Responsive Web Design
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


## jQuery, Events, and The DOM
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
