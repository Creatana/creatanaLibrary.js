# creatanaLibrary.js
Set of tools for accessing and modifying elements in HTML DOM

##Usage:

* Select the element with JavaScript:

  var element = document.getElementById('element-id');



* ######`getParentByClassName`
  Returns the 1st parent it finds with the class name.

  Example: `var parent = getParentByClassName(element, 'parent-class');`



* ######`realParentUp`
  If you're looking for a parent container holding many elements, not just 1. This will check the current, then check parents recursively for more than 1 child. Gets the first parent with more than 1 child.

  Example: `var parentAbove = realParentUp(parent);`



* ######`realParentDown`
  The opposite of `realParentUp`. Gets the first child element with more than 1 child

  Example: `var parentBelow = realParentDown(parent);`



* ######`realChild`
  Find the last element in a series of containers. Gets the last child.

  Example:
   ```
   var mediaContainer = document.getElementById('media-container-X');
   var media = realChild(mediaContainer);
   ```



* ######`getAllParents`
  Get an array of all parent elements

  Example: `var allParents = getAllParents(element);`



* ######`addHTML`
  Add HTML above the previous HTML

  Example: `addHTML(parent, '<a href="http:\/\/www.example.com">Click Me<\/a>');`



* ######`insertClasses`
  Insert class names into any element

  Example: `insertClasses(element, 'class-name');`
  or
  `insertClasses(element, 'class-name-1 class-name-2');`



* ######`deleteClass`
  Delete class names from any element

  Example: `deleteClass(element, 'class-name');`

* ######`addToAttribute`
  Add onto an existing attribute or make a new one.

  Example: `addToAttribute(element, 'href', '#top');`



* ######`addStyle`
  Add a style directly to the element style tag

  Example: `addStyle(element, 'display', 'none');`
or
  `addStyle(element, 'display', 'none !important');`

