# 🚀 ES6 JavaScript Mastery Exercises

> Topic-by-topic ES6 JavaScript exercise plan to help you master ES6 step by step.

---

## 📚 Table of Contents

1. [let, const, and Block Scope](#1-let-const-and-block-scope)
2. [Template Literals](#2-template-literals)
3. [Arrow Functions](#3-arrow-functions)
4. [Default Parameters](#4-default-parameters)
5. [Destructuring Arrays](#5-destructuring-arrays)
6. [Destructuring Objects](#6-destructuring-objects)
7. [Rest Parameters](#7-rest-parameters)
8. [Spread Operator](#8-spread-operator)
9. [Enhanced Object Literals](#9-enhanced-object-literals)
10. [Classes](#10-classes)
11. [Modules: export and import](#11-modules-export-and-import)
12. [Promises](#12-promises)
13. [async and await](#13-async-and-await)
14. [Array Methods with ES6 Style](#14-array-methods-with-es6-style)
15. [Set](#15-set)
16. [Map](#16-map)
17. [Mini Projects](#mini-projects-to-combine-es6-skills)
18. [Study Plan](#best-practice-study-order)

---

## 1. let, const, and Block Scope

### Exercise 1: Fix the Scope Bug

**Task:** Rewrite this code using `let` so it prints `0`, `1`, `2` instead of `3`, `3`, `3`:

```javascript
for (var i = 0; i < 3; i++) {
  setTimeout(function () {
    console.log(i);
  }, 1000);
}
```

**Expected Output:**
```
0
1
2
```

---

### Exercise 2: Choose let or const

Create variables for:
- `name`
- `age`
- `isStudent`
- `score`

**Rules:**
- ✅ Use `const` if the value should not be reassigned
- ✅ Use `let` if the value may change

Then update only the variables that should logically change.

---

### Exercise 3: Block Scope Practice

Create an if block:

```javascript
if (true) {
  // declare a variable here
}
```

**Task:** Try to access the variable outside the block. Explain why it works or fails with `let`, `const`, and `var`.

---

## 2. Template Literals

### Exercise 1: Profile Sentence

**Setup:**
```javascript
const name = "Ali";
const job = "developer";
const country = "Sudan";
```

**Task:** Use a template literal to print:
```
Ali is a developer from Sudan.
```

---

### Exercise 2: Multi-Line Message

Create this message using template literals:

```
Hello Ali,

Welcome to JavaScript ES6.
Today we will practice template literals.

Good luck!
```

---

### Exercise 3: Simple Receipt

**Setup:**
```javascript
const item = "Laptop";
const price = 800;
const tax = 50;
```

**Task:** Print:
```
Item: Laptop
Price: $800
Tax: $50
Total: $850
```

---

## 3. Arrow Functions

### Exercise 1: Convert to Arrow Function

Convert this function to an arrow function:

```javascript
function add(a, b) {
  return a + b;
}
```

---

### Exercise 2: One-Line Arrow Function

Write an arrow function called `square` that returns the square of a number.

**Example:**
```javascript
square(5); // 25
```

---

### Exercise 3: Arrow Function with Array Methods

**Given:**
```javascript
const numbers = [1, 2, 3, 4, 5];
```

**Task:** Use `.map()` with an arrow function to create:
```javascript
[2, 4, 6, 8, 10]
```

---

### Exercise 4: Arrow Function and `this`

**Create:**
```javascript
const user = {
  name: "Ali",
  regularFunction: function () {
    console.log(this.name);
  },
  arrowFunction: () => {
    console.log(this.name);
  }
};
```

**Task:** Call both functions and explain the difference.

---

## 4. Default Parameters

### Exercise 1: Greeting Function

**Task:** Write a function `greet(name)` that prints:
- `"Hello, Ali"` if name is provided
- `"Hello, Guest"` if no name is provided

**Examples:**
```javascript
greet("Ali");  // Hello, Ali
greet();       // Hello, Guest
```

---

### Exercise 2: Discount Calculator

**Task:** Create a function `calculatePrice(price, discount = 0)` that returns the final price after discount.

**Examples:**
```javascript
calculatePrice(100, 20); // 80
calculatePrice(100);     // 100
```

---

### Exercise 3: User Role

**Task:** Create a function `createUser(name, role = "member")` that returns:
```javascript
"Ali is a member"
"Sarah is an admin"
```

---

## 5. Destructuring Arrays

### Exercise 1: Basic Array Destructuring

**Given:**
```javascript
const colors = ["red", "green", "blue"];
```

**Task:** Use destructuring to create:
- `firstColor`
- `secondColor`
- `thirdColor`

---

### Exercise 2: Skip Values

**Given:**
```javascript
const numbers = [10, 20, 30, 40];
```

**Task:** Use destructuring to get only:
```javascript
10 // first
30 // third
```

---

### Exercise 3: Swap Variables

**Given:**
```javascript
let a = 5;
let b = 10;
```

**Task:** Use array destructuring to swap the values.

**Expected Result:**
```javascript
a = 10
b = 5
```

---

## 6. Destructuring Objects

### Exercise 1: Basic Object Destructuring

**Given:**
```javascript
const student = {
  name: "Ali",
  age: 25,
  course: "JavaScript"
};
```

**Task:** Use destructuring to extract `name`, `age`, and `course`.

---

### Exercise 2: Rename Variables

**Given:**
```javascript
const product = {
  title: "Phone",
  price: 500
};
```

**Task:** Use destructuring to create:
- `productTitle`
- `productPrice`

---

### Exercise 3: Default Values

**Given:**
```javascript
const user = {
  username: "coder123"
};
```

**Task:** Use destructuring so that:
```javascript
username = "coder123"
role = "guest"  // default value
```

---

## 7. Rest Parameters

### Exercise 1: Sum All Numbers

**Task:** Write a function `sum(...numbers)` that returns the total of all numbers.

**Examples:**
```javascript
sum(1, 2, 3);       // 6
sum(5, 10, 15, 20); // 50
```

---

### Exercise 2: Collect Extra Arguments

**Task:** Write a function `showSkills(name, ...skills)`.

**Example:**
```javascript
showSkills("Ali", "HTML", "CSS", "JavaScript");
// Expected: Ali knows HTML, CSS, JavaScript
```

---

### Exercise 3: Average Function

**Task:** Write a function `average(...scores)` that returns the average score.

---

## 8. Spread Operator

### Exercise 1: Copy an Array

**Given:**
```javascript
const original = [1, 2, 3];
```

**Task:** Use spread to create a copy. Then add `4` to the copy only.

**Expected:**
```javascript
original = [1, 2, 3]
copy = [1, 2, 3, 4]
```

---

### Exercise 2: Merge Arrays

**Given:**
```javascript
const frontend = ["HTML", "CSS"];
const backend = ["Node", "Express"];
```

**Task:** Use spread to create:
```javascript
["HTML", "CSS", "Node", "Express"]
```

---

### Exercise 3: Copy an Object

**Given:**
```javascript
const user = {
  name: "Ali",
  age: 30
};
```

**Task:** Use spread to copy the object and add `country: "Sudan"`.

---

### Exercise 4: Update Object Property

**Given:**
```javascript
const settings = {
  theme: "light",
  fontSize: 16
};
```

**Task:** Use spread to create a new object where `theme` is `"dark"`.

---

## 9. Enhanced Object Literals

### Exercise 1: Property Shorthand

**Given:**
```javascript
const name = "Ali";
const age = 30;
```

**Task:** Create an object using property shorthand:
```javascript
{
  name: "Ali",
  age: 30
}
```

---

### Exercise 2: Method Shorthand

**Create:**
```javascript
const calculator = {
  add(a, b) {
    return a + b;
  }
};
```

**Task:** Add methods for:
- `subtract`
- `multiply`
- `divide`

---

### Exercise 3: Computed Property Names

**Given:**
```javascript
const key = "email";
const value = "ali@example.com";
```

**Task:** Create an object that becomes:
```javascript
{
  email: "ali@example.com"
}
```

---

## 10. Classes

### Exercise 1: Create a Person Class

**Task:** Create a `Person` class with:
- Properties: `name`, `age`
- Method: `introduce()`

**Expected:**
```javascript
const person = new Person("Ali", 30);
person.introduce(); // My name is Ali and I am 30 years old.
```

---

### Exercise 2: Create a Student Class

**Task:** Create a `Student` class that extends `Person` with:
- Property: `course`
- Method: `study()`

**Expected Output:**
```
Ali is studying JavaScript.
```

---

### Exercise 3: Bank Account Class

**Task:** Create a `BankAccount` class with:
- Properties: `owner`, `balance`
- Methods: `deposit(amount)`, `withdraw(amount)`, `getBalance()`
- Validation: User cannot withdraw more than the balance

---

## 11. Modules: export and import

### Exercise 1: Export a Function

**Task:**
- Create `math.js` and export `add` and `subtract` functions
- Import them in `app.js`

---

### Exercise 2: Default Export

**Task:**
- Create `user.js` with default export for `createUser(name)` function
- Import it in another file

---

### Exercise 3: Utility Module

**Task:**
- Create `stringUtils.js` and export:
  - `capitalize()`
  - `reverseString()`
  - `countCharacters()`
- Use them in `app.js`

---

## 12. Promises

### Exercise 1: Basic Promise

**Task:** Create a promise that resolves after 2 seconds with `"Data loaded"`. Then print the message using `.then()`.

---

### Exercise 2: Promise Rejection

**Task:** Create a promise that rejects with `"Something went wrong"`. Catch the error using `.catch()`.

---

### Exercise 3: Simulate Login

**Task:** Create a function `login(username, password)` that:
- **Resolves** with `"Login successful"` if username is `"admin"` and password is `"1234"`
- **Rejects** with `"Invalid credentials"` otherwise

---

## 13. async and await

### Exercise 1: Convert Promise to Async/Await

**Task:** Use the promise from the previous section and consume it using an `async` function with `await`.

---

### Exercise 2: Try/Catch with Async

**Task:** Create an async function that calls `login()`. Use `try`/`catch` to handle success and failure.

---

### Exercise 3: Fake API Call

**Task:** Create a function `fetchUser()` that returns a promise resolving with:

```javascript
{
  id: 1,
  name: "Ali",
  role: "developer"
}
```

**Expected:** Use async/await to print:
```
User Ali is a developer.
```

---

## 14. Array Methods with ES6 Style

### Exercise 1: map

**Given:**
```javascript
const prices = [10, 20, 30];
```

**Task:** Create `[20, 40, 60]` (double each value)

---

### Exercise 2: filter

**Given:**
```javascript
const ages = [12, 18, 25, 30, 15];
```

**Task:** Create an array of adults only.

**Expected:**
```javascript
[18, 25, 30]
```

---

### Exercise 3: reduce

**Given:**
```javascript
const cart = [
  { item: "Book", price: 20 },
  { item: "Pen", price: 5 },
  { item: "Bag", price: 50 }
];
```

**Task:** Use `reduce` to calculate the total price.

---

### Exercise 4: find

**Given:**
```javascript
const users = [
  { id: 1, name: "Ali" },
  { id: 2, name: "Sarah" },
  { id: 3, name: "Omar" }
];
```

**Task:** Find the user with `id: 2`.

---

## 15. Set

### Exercise 1: Remove Duplicates

**Given:**
```javascript
const numbers = [1, 2, 2, 3, 4, 4, 5];
```

**Task:** Use `Set` to create:
```javascript
[1, 2, 3, 4, 5]
```

---

### Exercise 2: Unique Skills

**Given:**
```javascript
const skills = ["HTML", "CSS", "HTML", "JavaScript", "CSS"];
```

**Task:** Create a unique skills array.

---

### Exercise 3: Check Membership

**Task:** Create a Set of allowed roles:
- `admin`
- `editor`
- `viewer`

Check whether `"admin"` exists.

---

## 16. Map

### Exercise 1: Store User Scores

**Task:** Create a Map where:
- Ali => 90
- Sarah => 85
- Omar => 75

Print Sarah's score.

---

### Exercise 2: Update a Map Value

**Task:** Increase Ali's score by 5.

---

### Exercise 3: Loop Through Map

**Task:** Print each name and score:
```
Ali scored 95
Sarah scored 85
Omar scored 75
```

---

## Mini Projects to Combine ES6 Skills

### Project 1: Student Grade Manager

**Concepts Used:**
- `const` / `let`
- Array methods
- Objects
- Template literals
- Arrow functions
- Destructuring

**Setup:**
```javascript
const students = [
  { name: "Ali", grade: 90 },
  { name: "Sarah", grade: 75 },
  { name: "Omar", grade: 60 },
  { name: "Lina", grade: 95 }
];
```

**Tasks:**
1. Print each student's name and grade
2. Find students who passed (grade >= 60)
3. Calculate average grade
4. Find the top student
5. Create a new array with messages:
   ```
   Ali scored 90
   Sarah scored 75
   ```

---

### Project 2: Shopping Cart

**Concepts Used:**
- Classes
- Array methods
- Spread operator
- Destructuring
- Template literals

**Requirements:**
- Create a cart system with methods:
  - `addItem()`
  - `removeItem()`
  - `getTotal()`
  - `applyDiscount()`
  - `printReceipt()`

**Example Item:**
```javascript
{
  name: "Keyboard",
  price: 50,
  quantity: 2
}
```

---

### Project 3: Fake User API

**Concepts Used:**
- Promises
- async/await
- try/catch
- Destructuring
- Template literals

**Fake Data:**
```javascript
const users = [
  { id: 1, name: "Ali", role: "admin" },
  { id: 2, name: "Sarah", role: "editor" },
  { id: 3, name: "Omar", role: "viewer" }
];
```

**Create Functions:**
- `fetchUsers()`
- `fetchUserById(id)`
- `displayUser(id)`

**Expected Output:**
```
User Sarah has role editor.
```

---

### Project 4: ES6 Contact Manager

**Concepts Used:**
- Classes
- Map
- Set
- Spread operator
- Destructuring
- Template literals

**Requirements:**
- Add a contact
- Remove a contact
- Search by name
- List all contacts
- Prevent duplicate phone numbers using Set

**Example Contact:**
```javascript
{
  name: "Ali",
  phone: "123456",
  email: "ali@example.com"
}
```

---

## Best Practice Study Order

### 📖 Recommended Sequence

1. ✅ **let, const, block scope**
2. ✅ **Template literals**
3. ✅ **Arrow functions**
4. ✅ **Destructuring** (arrays & objects)
5. ✅ **Spread and rest operators**
6. ✅ **Array methods**
7. ✅ **Objects and enhanced object literals**
8. ✅ **Classes**
9. ✅ **Modules**
10. ✅ **Promises**
11. ✅ **Async/await**
12. ✅ **Set and Map**
13. ✅ **Mini projects**

---

### 🎯 5-Day Mastery Pattern

For each topic, follow this 5-day learning cycle:

| Day | Activity |
|-----|----------|
| **Day 1** | 📚 Read the concept |
| **Day 2** | 💪 Solve 3 small exercises |
| **Day 3** | 🚀 Solve 1 mini challenge |
| **Day 4** | 🗣️ Explain the topic out loud |
| **Day 5** | 🔨 Rebuild without looking |

---

## 🔥 Most Important ES6 Skills (Priority)

Master these first—they appear constantly in React, Node.js, APIs, and coding interviews:

1. **const / let** - Variable declaration and scoping
2. **Arrow functions** - Concise function syntax
3. **Template literals** - String interpolation
4. **Destructuring** - Extract values from arrays/objects
5. **Spread/Rest operators** - Array and object manipulation
6. **Array methods** - map, filter, reduce, find
7. **async/await** - Asynchronous programming

---

## 📝 Quick Reference

| Concept | Why It Matters |
|---------|----------------|
| `const`/`let` | Better scoping, fewer bugs |
| Arrow functions | Cleaner syntax, consistent `this` binding |
| Template literals | Readable string interpolation |
| Destructuring | Extract values elegantly |
| Spread/Rest | Flexible function arguments & object cloning |
| Array methods | Functional programming paradigm |
| Classes | OOP in JavaScript |
| async/await | Easy asynchronous code |

---

## 🎓 Tips for Success

- 💡 **Practice consistently** - Small, daily practice beats cramming
- 🧪 **Experiment** - Try variations and edge cases
- 📖 **Read others' code** - Learn different patterns
- 🐛 **Debug actively** - Use console logs and dev tools
- 🤝 **Discuss concepts** - Explain to others or your rubber duck
- 🏗️ **Build projects** - Apply multiple concepts together

---

## 📚 Resources

- [MDN Web Docs - ES6](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference)
- [JavaScript.info - Modern JavaScript](https://javascript.info/)
- [ES6 Features Overview](https://es6-features.org/)

---

**Happy Learning! 🚀 Master ES6 one concept at a time.**
