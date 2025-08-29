Q1 What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?
 Answer: getElementById() selects only one element by its unique ID and always returns a single element.
 getElementByClassName() selects one or more elements by their class name. It returns an HTML collection, which is a live collection. This means if the DOM changes, the collection is automatically updated.
 querySelector() selects the first element that matches a given CSS selector (it can be an ID, class, tag, or attribute). It always returns single element.
 querySelectorAll() selects all that match a given CSS selector and returns a static NodeList.

Q2 How do you create and insert a new element into the DOM?
 Answer: To create and insert a new element into the DOM, we use two main steps:
 1. Create the element using document.createElement("tagName")
 2. Insert the element into the DOM using methods like appendChild(), append(), prepend() or insertBefore().

Q3 What is Event Bubbling and how does it work?
Answer: Event Bubbling is the process in the DOM where an event starts from the target element (the element that was actually clicked or interacted with) and bubbles up to its parent elements, continuing until it reaches the root (documenet)

Q4 What is Event Delegation in JavaScript? Why is it useful?
Answer: Event Delegation is a technique is JS where instead of adding event listeners to multiple child elements we add a single event listener to a parent element. Because of event bubbling, when an event happens on a child element, it bubbles up to the parent, and the parent's event listener can handle it. This allows is to manage events efficiently, especially when dealing with a large number of elements or dynamically created elements.

Q5 What is the difference between preventDefault() and stopPropagation() methods?
Answer: preventDefault() stops the element's default behaviour. Such as, link navigation, form submition.
stopPropagation() stops the event form bubbling up to parent elements.
