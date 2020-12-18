# Retro 1: 301-retro.md

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
