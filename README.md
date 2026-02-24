1. What is the difference between getElementById, getElementsByClassName, and querySelector / querySelectorAll?

1. getElementById()
#Returns single element
#Fastest method
#Only works with id

2. getElementsByClassName()
#Returns HTMLCollection
#Can return multiple elements
#Must use index to access

3. querySelector()
#Returns first matched element
#Uses full CSS selector power
#Returns null if not found


4. querySelectorAll()
#Returns NodeList
#Static collection
#Supports for Each
#flexible

<!-- ................................................ -->

2. How do you create and insert a new element into the DOM?

DOM using JavaScript, you typically use document.createElement() to create the element and then methods like appendChild(), append(), prepend() 

<!-- ................................................. -->

3. What is Event Bubbling? And how does it work?

Event Bubbling is a mechanism in the browser's Document Object Model (DOM) where an event—such as a click or keypress—starts at the specific "target" element and then propagates upward through its ancestors in the DOM tree.

document.getElementById("parent").addEventListener("click", () => {
  console.log("Parent clicked");
});

document.getElementById("child").addEventListener("click", () => {
  console.log("Child clicked");
});
<!-- ............................................... -->

4. What is Event Delegation in JavaScript? Why is it useful?


a JavaScript technique that leverages event bubbling to efficiently manage events for many elements with a single event listener on a parent element

When an event (like a click) occurs on a child element, it "bubbles up" through its ancestors, allowing the parent's listener to catch it

<!-- ............................................................ -->

5. What is the difference between preventDefault() and stopPropagation() methods?


event.preventDefault() stops the browser's default action for an event.

stopPropagation() stops the event from propagating through the DOM.

<!-- .......................................................... -->