## Name some key differences between a Syntax Error and a Logic Error

Syntax errors are when there are spelling errors in your code that cause the program to not run, or stop part way through. These usually are okay to fix as long as you know what the error message means.

Logic errors are when the syntax is correct but the code is not what the user intended it to be, meaning the program runs successfully but gives incorrect results.

## List a few types of errors that you have encountered in past lab assignments and explain how you were able to correct them

I remember getting a couple of syntax errors when i was running the function to produce results with a random number generator but I hadn't appended the right element in my code somewheere, and then I had a declaration that wasn't being read because it was inside of a whole different function.

## How will this topic continue to influence your long term goals?

It teaches me to be aware of what kind of mistakes that's possible to make in writing and reading my code.

## How would you describe the JavaScript Debugger tool and how it works to someone just starting out in software development?

The debugger allows you to watch the flow of your code and if you want to put pauses in certain places in your code to see what is preventing it from running properly.

## Define what a breakpoint is

A breakpoint is when you place a pause in your code to allow you to identify what problems may occur to prevent you from running your code properly.

## What is the call stack?

The call stack is a section that shows you what code was executed to get to the current line.



## Assume you are in a pair programming session, and are the navigator. Your driver for this exercise will be a chatbot of your choice. 
For each of the lines of code below, provide the (nerdy) english instructions that you would describe to the chatbot so that it will return the code shown.

For example, if you wanted the chatbot to return this code:

const number = parseInt("2");
You would say:

Use JS to declare a variable called number and assign it the return value from running the parseInt function with the argument "2"

JavaScript Objects
const character = {
  name: 'Mario',
  age: 35,
  occupation: 'Plumber',
  powerUps: ['Super Mushroom', 'Fire Flower', 'Starman'],
  getBio: function() {
    return `${this.name} is a ${this.age}-year-old ${this.occupation} who has the following power-ups: ${this.powerUps.join(", ")}.`;
  }
};


1: Use JS code to declare an object literal  called "character" with various properties.
// It has a name, age, occupation, powerUps, and a getBio function.

console.log(character.name);



 2: Output the value of the "name" property of the "character" object to the console.

const keyword = 'powerUps';



console.log(character[keyword][1]);

 3: Output the second element of the "powerUps" array (using the value stored in the "keyword" variable) to the console.

const props = ['name', 'age', 'occupation', 'powerUps', 'getBio'];
for (let i = 0; i < props.length; i++) {
  console.log(props[i], character[props[i]]);
}

4: Iterate over each element in the "props" array.
// Output the property name and its corresponding value from the "character" object to the console.

// Functions
function sayHi(name) {
  console.log('Hi', name);
}

5: Define a function called "sayHi" that takes a parameter called "name".
// It outputs a greeting message along with the provided name.

const screamHello = function(name) {
  console.log('HELLO', name.toUpperCase());
}

 6: Define an anonymous function assigned to the "screamHello" variable.
// It takes a parameter called "name" and outputs a greeting message in uppercase.

sayHi('Ada');

7: Invoke the "sayHi" function and pass the string 'Ada' as an argument.
// It will output the greeting message 'Hi Ada' to the console.

screamHello('Victor');

 8: Invoke the "screamHello" function and pass the string 'Victor' as an argument.
// It will output the greeting message 'HELLO VICTOR' (in uppercase) to the console.

// Constructors
function Person(name) {
  this.fullName = name;
}

 9: Define a constructor function called "Person" that takes a parameter called "name".
// It sets the "fullName" property of the newly created object to the provided name.

Person.prototype.sayMyName = function() {
  console.log(this.fullName.toUpperCase());
};

 10: Add a method called "sayMyName" to the prototype of the "Person" constructor function.
// It outputs the value of the "fullName" property of the object (using "this") in uppercase.

Person.whisper = function() {
  console.log('sssshhhh');
};

 11: Add a static method called "whisper" to the "Person" constructor function.
// It outputs the message 'sssshhhh' to the console.

Person.sayMyName();

 12: Invoke the "sayMyName" method directly on the "Person" constructor function.
// Since it is a static method, it is not available on individual instances.

const ada = new Person('Ada Lovelace');
ada.sayMyName();

// Step the "ada" variable.
// The "fullName" property is set to 'Ada Lovelace'.
// Invoke the "sayMyName" method on the "ada" object.
// It will output 'ADA LOVELACE' (in uppercase) to the console.

ada.whisper();

14: Invoke the "whisper" static method directly on the "Person" constructor function.
// It will output the message 'sssshhhh' to the console.

Person.whisper();
