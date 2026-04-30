Topic-by-topic ES6 JavaScript exercise plan to help you master ES6 step by step.

ES6 JavaScript Mastery Exercises
1. let, const, and Block Scope



Exercise 1: Fix the Scope Bug
for (var i = 0; i < 3; i++) {
  setTimeout(function () {
    console.log(i);
  }, 1000);
}
Task: Rewrite it using let so it prints:
0
1
2


Exercise 2: Choose let or const
Create variables for:
name
age
isStudent
score
Rules:
•	Use const if the value should not be reassigned.
•	Use let if the value may change.
Then update only the variables that should logically change.
Exercise 3: Block Scope Practice
Create an if block:
if (true) {
  // declare a variable here
}

Try to access the variable outside the block.
Task: Explain why it works or fails with let, const, and var.
________________________________________
2. Template Literals
Exercise 1: Profile Sentence
Create variables:
const name = "Ali";
const job = "developer";
const country = "Sudan";
Use a template literal to print:
Ali is a developer from Sudan.
Exercise 2: Multi-Line Message
Create this message using template literals:
Hello Ali,

Welcome to JavaScript ES6.
Today we will practice template literals.

Good luck!
Exercise 3: Simple Receipt
Create variables:
const item = "Laptop";
const price = 800;
const tax = 50;
Print:
Item: Laptop
Price: $800
Tax: $50
Total: $850
________________________________________
3. Arrow Functions
Exercise 1: Convert to Arrow Function
Convert this function:
function add(a, b) {
  return a + b;
}
Into an arrow function.
Exercise 2: One-Line Arrow Function
Write an arrow function called square that returns the square of a number.
Example:
square(5); // 25
Exercise 3: Arrow Function with Array Methods
Given:
const numbers = [1, 2, 3, 4, 5];
Use .map() with an arrow function to create:
[2, 4, 6, 8, 10]
Exercise 4: Arrow Function and this
Create an object:
const user = {
  name: "Ali",
  regularFunction: function () {
    console.log(this.name);
  },
  arrowFunction: () => {
    console.log(this.name);
  }
};
Task: Call both functions and explain the difference.
________________________________________
4. Default Parameters
Exercise 1: Greeting Function
Write a function:
greet(name)
If no name is provided, it should print:
Hello, Guest
Example:
greet("Ali"); // Hello, Ali
greet();      // Hello, Guest
Exercise 2: Discount Calculator
Create a function:
calculatePrice(price, discount = 0)
It should return the final price after discount.
Example:
calculatePrice(100, 20); // 80
calculatePrice(100);     // 100
Exercise 3: User Role
Create a function:
createUser(name, role = "member")
It should return:
"Ali is a member"
"Sarah is an admin"
________________________________________
5. Destructuring Arrays
Exercise 1: Basic Array Destructuring
Given:
const colors = ["red", "green", "blue"];
Use destructuring to create:
firstColor
secondColor
thirdColor
Exercise 2: Skip Values
Given:
const numbers = [10, 20, 30, 40];
Use destructuring to get only:
10
30
Exercise 3: Swap Variables
Given:
let a = 5;
let b = 10;
Use array destructuring to swap the values.
Expected:
a = 10
b = 5
________________________________________
6. Destructuring Objects
Exercise 1: Basic Object Destructuring
Given:
const student = {
  name: "Ali",
  age: 25,
  course: "JavaScript"
};
Use destructuring to extract:
name
age
course
Exercise 2: Rename Variables
Given:
const product = {
  title: "Phone",
  price: 500
};
Use destructuring to create:
productTitle
productPrice
Exercise 3: Default Values
Given:
const user = {
  username: "coder123"
};
Use destructuring so that:
username = "coder123"
role = "guest"
________________________________________
7. Rest Parameters
Exercise 1: Sum All Numbers
Write a function:
sum(...numbers)
It should return the total of all numbers.
Example:
sum(1, 2, 3);       // 6
sum(5, 10, 15, 20); // 50
Exercise 2: Collect Extra Arguments
Write a function:
showSkills(name, ...skills)
Example:
showSkills("Ali", "HTML", "CSS", "JavaScript");
Expected output:
Ali knows HTML, CSS, JavaScript
Exercise 3: Average Function
Write a function:
average(...scores)
It should return the average score.
________________________________________
8. Spread Operator
Exercise 1: Copy an Array
Given:
const original = [1, 2, 3];
Use spread to create a copy.
Then add 4 to the copy only.
Expected:
original = [1, 2, 3]
copy = [1, 2, 3, 4]
Exercise 2: Merge Arrays
Given:
const frontend = ["HTML", "CSS"];
const backend = ["Node", "Express"];
Use spread to create:
["HTML", "CSS", "Node", "Express"]
Exercise 3: Copy an Object
Given:
const user = {
  name: "Ali",
  age: 30
};
Use spread to copy the object and add:
country: "Sudan"
Exercise 4: Update Object Property
Given:
const settings = {
  theme: "light",
  fontSize: 16
};
Use spread to create a new object where:
theme: "dark"
________________________________________
9. Enhanced Object Literals
Exercise 1: Property Shorthand
Given:
const name = "Ali";
const age = 30;
Create an object using property shorthand:
{
  name: "Ali",
  age: 30
}
Exercise 2: Method Shorthand
Create an object:
const calculator = {
  add(a, b) {
    return a + b;
  }
};
Add methods for:
subtract
multiply
divide
Exercise 3: Computed Property Names
Given:
const key = "email";
const value = "ali@example.com";
Create an object that becomes:
{
  email: "ali@example.com"
}
________________________________________
10. Classes
Exercise 1: Create a Person Class
Create a class:
class Person
With:
name
age
introduce()
Expected:
const person = new Person("Ali", 30);
person.introduce(); // My name is Ali and I am 30 years old.
Exercise 2: Create a Student Class
Create a class Student that extends Person.
Add:
course
study()
Expected:
Ali is studying JavaScript.
Exercise 3: Bank Account Class
Create a class:
class BankAccount
With:
owner
balance
deposit(amount)
withdraw(amount)
getBalance()
Add validation so the user cannot withdraw more than the balance.
________________________________________
11. Modules: export and import
Exercise 1: Export a Function
Create a file:
math.js
Export:
add
subtract
Import them in:
app.js
Exercise 2: Default Export
Create:
user.js
Default export a function:
createUser(name)
Import it in another file.
Exercise 3: Utility Module
Create a file:
stringUtils.js
Export:
capitalize()
reverseString()
countCharacters()
Use them in app.js.
________________________________________
12. Promises
Exercise 1: Basic Promise
Create a promise that resolves after 2 seconds with:
"Data loaded"
Then print the message using .then().
Exercise 2: Promise Rejection
Create a promise that rejects with:
"Something went wrong"
Catch the error using .catch().
Exercise 3: Simulate Login
Create a function:
login(username, password)
If username is "admin" and password is "1234", resolve:
"Login successful"
Otherwise reject:
"Invalid credentials"
________________________________________
13. async and await
Exercise 1: Convert Promise to Async/Await
Use the promise from the previous section and consume it using:
async function loadData()
Use await.
Exercise 2: Try/Catch with Async
Create an async function that calls login().
Use:
try
catch
To handle success and failure.
Exercise 3: Fake API Call
Create a function:
fetchUser()
It returns a promise that resolves with:
{
  id: 1,
  name: "Ali",
  role: "developer"
}
Use async/await to print:
User Ali is a developer.
________________________________________
14. Array Methods with ES6 Style
Exercise 1: map
Given:
const prices = [10, 20, 30];
Create:
[20, 40, 60]
Exercise 2: filter
Given:
const ages = [12, 18, 25, 30, 15];
Create an array of adults only.
Expected:
[18, 25, 30]
Exercise 3: reduce
Given:
const cart = [
  { item: "Book", price: 20 },
  { item: "Pen", price: 5 },
  { item: "Bag", price: 50 }
];
Use reduce to calculate the total price.
Exercise 4: find
Given:
const users = [
  { id: 1, name: "Ali" },
  { id: 2, name: "Sarah" },
  { id: 3, name: "Omar" }
];
Find the user with id: 2.
________________________________________
15. Set
Exercise 1: Remove Duplicates
Given:
const numbers = [1, 2, 2, 3, 4, 4, 5];
Use Set to create:
[1, 2, 3, 4, 5]
Exercise 2: Unique Skills
Given:
const skills = ["HTML", "CSS", "HTML", "JavaScript", "CSS"];
Create a unique skills array.
Exercise 3: Check Membership
Create a Set of allowed roles:
admin
editor
viewer
Check whether "admin" exists.
________________________________________
16. Map
Exercise 1: Store User Scores
Create a Map where:
Ali => 90
Sarah => 85
Omar => 75
Print Sarah’s score.
Exercise 2: Update a Map Value
Increase Ali’s score by 5.
Exercise 3: Loop Through Map
Print each name and score:
Ali scored 95
Sarah scored 85
Omar scored 75
________________________________________
Mini Projects to Combine ES6 Skills
Project 1: Student Grade Manager
Use:
const
let
array methods
objects
template literals
arrow functions
destructuring
Create an array:
const students = [
  { name: "Ali", grade: 90 },
  { name: "Sarah", grade: 75 },
  { name: "Omar", grade: 60 },
  { name: "Lina", grade: 95 }
];
Tasks:
1.	Print each student’s name and grade.
2.	Find students who passed.
3.	Calculate average grade.
4.	Find the top student.
5.	Create a new array with messages:
Ali scored 90
Sarah scored 75
________________________________________
Project 2: Shopping Cart
Use:
classes
array methods
spread
destructuring
template literals
Create a cart system with:
addItem()
removeItem()
getTotal()
applyDiscount()
printReceipt()
Example item:
{
  name: "Keyboard",
  price: 50,
  quantity: 2
}
________________________________________
Project 3: Fake User API
Use:
Promise
async/await
try/catch
destructuring
template literals
Create:
fetchUsers()
fetchUserById(id)
displayUser(id)
Fake data:
const users = [
  { id: 1, name: "Ali", role: "admin" },
  { id: 2, name: "Sarah", role: "editor" },
  { id: 3, name: "Omar", role: "viewer" }
];
Expected:
User Sarah has role editor.
________________________________________
Project 4: ES6 Contact Manager
Use:
class
Map
Set
spread
destructuring
template literals
Create a contact manager that can:
1.	Add a contact.
2.	Remove a contact.
3.	Search by name.
4.	List all contacts.
5.	Prevent duplicate phone numbers using Set.
Example contact:
{
  name: "Ali",
  phone: "123456",
  email: "ali@example.com"
}
________________________________________
Best Practice Study Order
Follow this order:
1.	let, const, block scope
2.	Template literals
3.	Arrow functions
4.	Destructuring
5.	Spread and rest
6.	Array methods
7.	Objects and enhanced object literals
8.	Classes
9.	Modules
10.	Promises
11.	Async/await
12.	Set and Map
13.	Mini projects
For mastery, do each topic like this:
Day 1: Read the concept
Day 2: Solve 3 small exercises
Day 3: Solve 1 mini challenge
Day 4: Explain the topic out loud
Day 5: Rebuild without looking


The most important ES6 skills to master first are:
const / let
arrow functions
template literals
destructuring
spread/rest
array methods
async/await
These appear constantly in React, Node.js, APIs, and coding interviews.

