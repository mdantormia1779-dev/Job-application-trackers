1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
Ans:
 
getElementById()
getElementById selects a single element using its unique id.
example: document.getElementById("card");

getElementsByClassName()
getElementByClassName() selects multiple elements using a class name t returns an HTMLCollection, which looks like an array but is not a real array.
it is a live collection meaning if the DOM changes the collection updates automatically.
example: document.getElementsByClassName('card');

querySelector()
querySelector() selects the first matching element using a css selector .
we can use id, class, tag name, css selector 
example: document.querySelector(".card");

querySelectorAll()
querySelectorAll() selects all matching elements using a CSS selector.
it returns a NodeList which supports method like forEach().

2. How do you create and insert a new element into the DOM?
Ans:
create a new element,add content to the element insert into the DOM
const div=document.createElement("div");
div.innerText="Hello World";
document.body.appendChild(div);

3. What is Event Bubbling? And how does it work?
Ans:
Event Bubbling is a process where an event starts from the target element and and then propagates
(moves upward) to its parent grandparent and up to the document.

4. What is Event Delegation in JavaScript? Why is it useful?
Ans:
Event Delegation is a technique where you attach an event listener to a parent element instead
of adding separate listeners to multiple child elements.
it is useful because:
    it reduces the amount of code.
    it improves performance.
    it works for dynamically created elements.
    it makes the code clener and easier to manage.

5. What is the difference between preventDefault() and stopPropagation() methods?
Ans:
preventDefault() stops the default behavior of an element.
for example, it prevents a form from submitting or a link from navigating.

stopPropagation()
stopPropagation() stops the event from bubbling up to parent elements.


 
