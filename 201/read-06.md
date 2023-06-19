
## How would you describe an object to a non-technical friend you grew up with?
a collection of information that has functions or equations related to it.

## What are some advantages to creating object literals?

convenience, flexibility in declaration, and less code during declaration. You can drop an object literal anywhere in your program with no previous setup and it'll work, which can be very handy!

## How do objects differ from arrays?
arrays use numbers to access elements while objects use properties to access elements.

## Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation
When you need a person’s age or information in an address

## Evaluate the code below. What does the term this refer to and what is the advantage to using this?
This refers to the dog, it’s useful because if you have to create more than one this enables you to use the same method more than once.

const dog = { name: ‘Spot’, age: 2, color: ‘white with black spots’, humanAge: function (){ console.log(${this.name} is ${this.age*7} in human years); } }

## What is the DOM?
The DOM is a programming interface for web documents, It represents the page so that programs can change the document structure, style, and content.

## Briefly describe the relationship between the DOM and JavaScript
he DOM (Document Object Model) is essentially the API one uses to manipulate an HTML (or XML) document -- usually using JavaScript, since that's the language we have in the browser,

As others have said, the DOM (Document Object Model) is essentially the API one uses to manipulate an HTML (or XML) document -- usually using JavaScript, since that's the language we have in the browser, but not always, as there are DOM-like APIs for manipulating these documents in other languages on the server side or the desktop.

JavaScript is just a programming language. It happens to be the de facto standard scripting language for most (if not all) web browsers, and so in practice, most of the time when you're writing DOM manipulation scripts to be run on the client side, you're working with both the DOM and JavaScript at the same time.

## Things I want to know more about