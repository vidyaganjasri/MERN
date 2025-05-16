# JavaScript Object Example: `person`

This project demonstrates how to use **JavaScript objects** to store and access data like a digital profile.

## 💡 What This Does

- Creates an object named `person` with details like name, age, hobbies, and address.
- Displays parts of the object using `console.log()` and `alert()`.
- Uses **object destructuring** to access values more easily.

## 🧠 Code Breakdown

```js
const person = {
    firstName: 'john',
    lastName: 'Doe',
    age: 30,
    hobbies: ['music', 'movies', 'sports'],
    address: {
        street: '50 main street',
        city: 'Boston',
        state: 'MA'
    }
}

alert("hi " + person.firstName);             // Popup: hi john
console.log(person.firstName);               // Logs: john
console.log(person.hobbies[1]);              // Logs: movies
console.log(person.address.street);          // Logs: 50 main street

const { firstName, lastName, address: { city } } = person;
console.log(firstName + ' ' + city);         // Logs: john Boston
```


# output
![image](https://github.com/user-attachments/assets/f0f1a27d-18df-4af7-861e-551164e62619)
![image](https://github.com/user-attachments/assets/a2d0ee03-c5ca-45fa-8fec-afedf2d691fa)



## 💡 What This Does
adds a property in an object
here is the following code: 
```
const person = {
    firstName:'john', 
    lastName:'Doe',
    age:30,
    hobbies: ['music','movies','sports'],
    address:{
        street: '50 main street',
        city: 'Boston',
        state:'MA'
    }
}

person.email = 'john@gmail.com';
console.log(person);
```
output 
![image](https://github.com/user-attachments/assets/e31aeecb-f2de-42d8-86e9-b6f08d907e2c)

# JavaScript Todo List Example

This project shows how to use an **array of objects** in JavaScript to represent a simple **to-do list**.

---

## 📌 What the Code Does

- Creates a list called `todo` that holds multiple task objects.
- Each task (or "todo item") includes:
  - `id`: A unique number for each task
  - `text`: A description of the task
  - `isCompleted`: A true/false value showing if the task is done
- Logs the full list to the browser console.

---

## 🧠 Code

```js
const todo = [
    {
        id: 1,
        text: 'Take out trash',
        isCompleted: true
    },
    {
        id: 2,
        text: 'Meeting with boss',
        isCompleted: true
    },
    {
        id: 3,
        text: 'Dentist appointment',
        isCompleted: true
    }
];

console.log(todo);
```
## output:
![image](https://github.com/user-attachments/assets/de1a1b0c-faa5-41cd-8ba6-c131612b88b1)

# Accessing a Specific Task from a JavaScript Todo List

This short example shows how to access and print a **specific field from a list of tasks** using JavaScript.

---

## 🧠 Code

```js
const todo = [
    {
        id: 1,
        text: 'Take out trash',
        isCompleted: true
    },
    {
        id: 2,
        text: 'Meeting with boss',
        isCompleted: true
    },
    {
        id: 3,
        text: 'Dentist appointment',
        isCompleted: true
    }
];

console.log(todo[1].text);
```

# 📦 Working with JSON in JavaScript

This project demonstrates how to **convert JavaScript objects into JSON** format — a key concept in full-stack development and APIs.

---

## 🧠 What is JSON?

**JSON** stands for **JavaScript Object Notation**.  
It’s a format for sending data — commonly used in:
- Full-stack development
- Web APIs
- Mobile apps
- Databases like MongoDB

---
## 🧩 Why Use JSON.stringify()?

- Converts JS objects to a format that can be sent to a backend or API.
- Easy to store in a file or database.
- Used in AJAX, Fetch, REST APIs, etc.

---

## 🔧 Code Example

```js
const todo = [
    {
        id: 1,
        text: 'Take out trash',
        isCompleted: true
    },
    {
        id: 2,
        text: 'Meeting with boss',
        isCompleted: true
    },
    {
        id: 3,
        text: 'Dentist appointment',
        isCompleted: true
    }
];

const todoJson = JSON.stringify(todo); // Convert to JSON string
console.log(todoJson);                 // Print the JSON string
```

# output 
![image](https://github.com/user-attachments/assets/ab4a8f8e-2c74-47c3-8b31-d2e174c81d84)


# JavaScript For Loop Example

This example demonstrates how to use a `for` loop to iterate over an array and log both the index and the item.

---

## Code

```js
for (let i = 0; i < todo.length; i++) {
    console.log(`For loop numbre: ${i}`);
    console.log(todo[i]);
}
```
# output: 
![image](https://github.com/user-attachments/assets/4ece941c-8285-4486-8fac-c7f1c2c995b6)

# Using Backticks `` ` `` vs Quotes `" "` in JavaScript Strings

---

## When to Use Backticks (Template Literals)

- Use **backticks** (`` ` ``) when you want to **include variables or expressions inside a string**.
- This is called a **template literal**.
- You insert variables using `${variableName}` syntax.

### Example:

```js
let i = 5;
console.log(`The number is ${i}`);  // Output: The number is 5
```

# Alternative method
```js
//for loops: 
for(let t of todo){
    console.log(t.text);
}
```

# output
![image](https://github.com/user-attachments/assets/f1b2e354-f3eb-4d23-9a6b-9d2516670c50)

# JavaScript Array Method: `forEach`

---

## Code Example

```js
todo.forEach(function(todo){
    console.log(todo.text);
});
```
## What is happening?

- The `forEach` method loops through each element in the `todo` array.

- For each item (`todo`), the function runs once.

- Inside the function, it prints the `text` property of the current `todo` object.

- This outputs the description of each task in the console.


# Using `.map()` to Extract an Array of Task Texts

---

## The Code

```js
// Returns an array of the text values from each todo item
const todoText = todo.map(function(todo){
    return todo.text;
});

console.log(todoText);
```
## What is happening?

- The `.map()` method creates a **new array** by transforming each element in the original `todo` array.

- The function inside `.map()` takes each `todo` object and returns its `text` property.

- As a result, `todoText` becomes an array containing only the text descriptions of all tasks.

- `console.log(todoText)` prints this new array, for example:
  

# Using `.filter()` and `.map()` to Get Completed Task Texts

---

## The Code

```js
// Filter tasks that are completed, then get their text
const todoCompleted = todo.filter(function(todo){
    return todo.isCompleted === true;
}).map(function(todo){
    return todo.text;
});

console.log(todoCompleted);
```
## What is happening?

- The code uses `.filter()` to create a new array containing only the tasks where `isCompleted` is `true`.
- Then, it uses `.map()` on the filtered array to extract just the `text` property from each completed task.
- The result is stored in the `todoCompleted` variable, which is an array of strings with the text of completed tasks.
- Finally, `console.log(todoCompleted)` prints this array to the console.

# Output of all the three 

![image](https://github.com/user-attachments/assets/80036c6d-19b7-40ed-bc1c-12cd34ff30a4)

