Concept Review
Assume you are in a pair programming session, and are the navigator. Your driver for this exercise will be a chatbot of your choice. For each of the lines of code below, provide the (nerdy) english instructions that you would describe to the chatbot so that it will return the code shown.

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
console.log(character.name);
const keyword = 'powerUps';
console.log(character[keyword][1]);
const props = ['name', 'age', 'occupation', 'powerUps', 'getBio'];
for( let i = 0; i < props.length; i++) {
  console.log( props[i],  character[props[i]]  );
}
Functions
function sayHi(name) {
  console.log('Hi', name);
}
const screamHello = function(name) {
  console.log( 'HELLO', name.toUpperCase() );
}
sayHi('Ada');
screamHello('Victor');
Constructors
function Person(name) {
  this.fullName = name;
}
Person.prototype.sayMyName = function() {
  console.log(this.fullName.toUpperCase());
}
Person.whisper = function() {
  console.log('sssshhhh');
}
Person.sayMyName();
const ada = new Person('Ada Lovelace');
ada.sayMyName();
ada.whisper();
Person.whisper();


// JavaScript Objects
const character = {
  name: 'Mario',
  age: 35,
  occupation: 'Plumber',
  powerUps: ['Super Mushroom', 'Fire Flower', 'Starman'],
  getBio: function() {
    return `${this.name} is a ${this.age}-year-old ${this.occupation} who has the following power-ups: ${this.powerUps.join(", ")}.`;
  }
};
console.log(character.name);
const keyword = 'powerUps';
console.log(character[keyword][1]);
const props = ['name', 'age', 'occupation', 'powerUps', 'getBio'];
for (let i = 0; i < props.length; i++) {
  console.log(props[i], character[props[i]]);
}

// Functions
function sayHi(name) {
  console.log('Hi', name);
}
const screamHello = function(name) {
  console.log('HELLO', name.toUpperCase());
}
sayHi('Ada');
screamHello('Victor');

// Constructors
function Person(name) {
  this.fullName = name;
}
Person.prototype.sayMyName = function() {
  console.log(this.fullName.toUpperCase());
};
Person.whisper = function() {
  console.log('sssshhhh');
};
Person.sayMyName();
const ada = new Person('Ada Lovelace');
ada.sayMyName();
ada.whisper();
Person.whisper();

// Step 1: Use JS code to declare an object literal  called "character" with various properties.
// It has a name, age, occupation, powerUps, and a getBio function.

console.log(character.name);

// Step 2: Output the value of the "name" property of the "character" object to the console.

const keyword = 'powerUps';



console.log(character[keyword][1]);

// Step 3: Output the second element of the "powerUps" array (using the value stored in the "keyword" variable) to the console.

const props = ['name', 'age', 'occupation', 'powerUps', 'getBio'];
for (let i = 0; i < props.length; i++) {
  console.log(props[i], character[props[i]]);
}

// Step 4: Iterate over each element in the "props" array.
// Output the property name and its corresponding value from the "character" object to the console.

// Functions
function sayHi(name) {
  console.log('Hi', name);
}

// Step 5: Define a function called "sayHi" that takes a parameter called "name".
// It outputs a greeting message along with the provided name.

const screamHello = function(name) {
  console.log('HELLO', name.toUpperCase());
}

// Step 6: Define an anonymous function assigned to the "screamHello" variable.
// It takes a parameter called "name" and outputs a greeting message in uppercase.

sayHi('Ada');

// Step 7: Invoke the "sayHi" function and pass the string 'Ada' as an argument.
// It will output the greeting message 'Hi Ada' to the console.

screamHello('Victor');

// Step 8: Invoke the "screamHello" function and pass the string 'Victor' as an argument.
// It will output the greeting message 'HELLO VICTOR' (in uppercase) to the console.

// Constructors
function Person(name) {
  this.fullName = name;
}

// Step 9: Define a constructor function called "Person" that takes a parameter called "name".
// It sets the "fullName" property of the newly created object to the provided name.

Person.prototype.sayMyName = function() {
  console.log(this.fullName.toUpperCase());
};

// Step 10: Add a method called "sayMyName" to the prototype of the "Person" constructor function.
// It outputs the value of the "fullName" property of the object (using "this") in uppercase.

Person.whisper = function() {
  console.log('sssshhhh');
};

// Step 11: Add a static method called "whisper" to the "Person" constructor function.
// It outputs the message 'sssshhhh' to the console.

Person.sayMyName();

// Step 12: Invoke the "sayMyName" method directly on the "Person" constructor function.
// Since it is a static method, it is not available on individual instances.

const ada = new Person('Ada Lovelace');
ada.sayMyName();

// Step 13: Create a new object using the "Person" constructor and assign it to the "ada" variable.
// The "fullName" property is set to 'Ada Lovelace'.
// Invoke the "sayMyName" method on the "ada" object.
// It will output 'ADA LOVELACE' (in uppercase) to the console.

ada.whisper();

// Step 14: Invoke the "whisper" static method directly on the "Person" constructor function.
// It will output the message 'sssshhhh' to the console.

Person.whisper();
