# JavaScript (JS)

JavaScript is a **programming language**.

## What You Can Do with JavaScript

JavaScript can be used for:
- **Front-end development**
- **Back-end development**
- **Full stack development**

## Initial Usage

- Originally used **only in browsers** to handle front-end interactions.

## Modern Usage

Today, JavaScript is used in:
- **Web applications**
- **Mobile apps**
- **Real-time networking applications** (e.g., chat apps)
- **Command line tools**
- **Games**

---

## Where Does JavaScript Run?

- Initially, JavaScript ran only in web **browsers**.
- Browsers have **JavaScript engines**:
  - Firefox: `SpiderMonkey`
  - Chrome: `V8`

### 2009: Node.js

- **Ryan Dahl** embedded Chrome's **V8 engine** in C++ to create **Node.js**.
- This allowed **JavaScript to run outside of the browser**.

---

## ECMAScript vs JavaScript

- **ECMAScript**: The **specification** or standard.
- **JavaScript**: The **language that follows** the ECMAScript specification.

---

# Commands

## Accessing the JavaScript Console

To run JavaScript in the browser:

1. Open **Chrome**.
2. Right-click anywhere on the page → Click **Inspect**.
3. Go to the **Console** tab.

![Console Image 1](https://github.com/user-attachments/assets/77446bc8-3e9e-49b3-9894-a4cb18b6acd2)

![Console Image 2](https://github.com/user-attachments/assets/56aecb99-22f7-4949-bf79-9dfe0e0ff5fd)

---

## Setting Up Development Environment

Recommended **code editors**:
- **VS Code**
- **Sublime Text**

### Set your environment as shown:

![Dev Env Setup](https://github.com/user-attachments/assets/03492717-a1c3-450f-926b-55f2ea5cc7a0)

---

## Placing JavaScript in HTML

You can include your JavaScript code in:
- The `<head>` section
- The `<body>` section

✅ **Best Practice**:  
Place your `<script>` tag at the **end of the body section**, just before the closing `</body>` tag.

> Reason:  
HTML is parsed **top to bottom**, and JavaScript code often interacts with body elements. If body elements are not yet loaded, the script may fail to work.

---

## Example

html
<script>
  console.log("Hello World");
</script>


# JavaScript Basics

- When **writing code in a script file**, all statements **should be terminated by a semicolon** (`;`).

- `"Hello World"` is a **string** in JavaScript.

- In JavaScript, `//` is used to write a **comment**.

  - Comments are **ignored by JavaScript** and **not executed**.

  - Comments are mainly used for **documentation**, explaining **why** something is done rather than **what** it does.


# How to See JavaScript Output

To look at the output of your JavaScript code:

- Open your **webpage** in a browser.
- Right-click anywhere on the page and select **Inspect**.
- Go to the **Console** tab to see the output.

Alternatively, you can use the keyboard shortcut:

- **Ctrl + Shift + I** (on Windows/Linux) or **Cmd + Option + I** (on Mac) to open the developer tools.
- Then go to the **Console** tab.

> Note:  
> The shortcut **Alt + Ctrl + I** might not work depending on your browser or system settings.

![image](https://github.com/user-attachments/assets/d83592e3-66b3-4f50-8d29-c21fae8b3d51)
![image](https://github.com/user-attachments/assets/8edc4321-6307-49c2-a252-a19ff896ef87)


Seperation of concerns to seperate html and js file 
still works
![image](https://github.com/user-attachments/assets/8db75296-483e-421d-9217-b28de305cf94)
![image](https://github.com/user-attachments/assets/28a0190d-26a7-435e-b7e4-40024d2a44c0)


![image](https://github.com/user-attachments/assets/d77e22d4-7ade-44a1-9709-e5046e6da8e9)


# Running JavaScript with Node.js

So far, we have run JavaScript code in the browser.

To run JavaScript using **Node.js**:

1. Open your terminal or command prompt.
2. Navigate to the directory where your JavaScript file (`file.js`) is saved using `cd` command.
3. Type the following command and press Enter:

   ```bash
   node file.js

![image](https://github.com/user-attachments/assets/0848165a-d86c-4ef6-92ce-1515cf2259f6)

# Running JavaScript with Node.js Inside VS Code

You can run your JavaScript files using Node.js **directly inside VS Code** without opening the command prompt separately.

Steps:

1. Open your JavaScript file in **VS Code**.
2. Open the **Integrated Terminal** in VS Code:
   - Use the shortcut: `` Ctrl + ` `` (backtick key)
   - Or go to **View > Terminal** from the menu.
3. In the terminal, make sure you are in the directory containing your JS file.
4. Run the file by typing:

   ```bash
   node file.js
   
![image](https://github.com/user-attachments/assets/7cae88ec-366d-411a-9917-a0353fdf0994)

# Variables

- A **variable** is used to store data temporarily in the computer's memory.
- Think of a variable as a **box**:  
  - The **label** on the box is the **name of the variable**.  
  - What’s inside the box is the **data**.
  - when we declare a var the value is **undefined**

## Declaring a Variable

```js
let name;
```

![image](https://github.com/user-attachments/assets/74c2365b-0e34-4810-9788-445ec7ceca21)


# Variable Naming Rules

- Variable names **should not** be reserved keywords like `let`, `if`, `var`, `else`, etc.
- Variable names **should be meaningful** (describe what they store).
- Variable names **cannot start with a number**.
- Variable names **cannot contain spaces or hyphens** (`-`).
- Variable names should follow **camelCase notation** (e.g., `firstName`).
- Variable names are **case-sensitive** (`name` and `Name` are different).

# Types of Declaration

You can declare multiple variables in one line:

```js
let firstName = "ganja", lastName = "vidya";
```

# Best Practice

Declare each variable on its own line for better readability:

```js
let firstName = 'ganja';
let lastName = 'vidya';
```

# Using `const` for Fixed Variables

- If you want your variable to be **fixed** (its value should not change), use `const` instead of `let`.

Example:

```js
const pi = 3.14;
```
![image](https://github.com/user-attachments/assets/89646836-ee9b-4672-9b77-2deb0eec4926)



# Types of Data Types

There are two main types of data types in JavaScript:

## 1. Primitive Types
- `string`
- `number`
- `boolean`
- `undefined`
- `null`

## 2. Reference Types
- objects
- array
- functions

![image](https://github.com/user-attachments/assets/f2d249cb-d2f7-40b0-aa98-c6be0d31eda1)

# JavaScript is a Dynamic Language

There are two types of typing in programming languages:

- **Static Typing:**  
  Variables have a fixed type that **cannot be changed** after declaration.

- **Dynamic Typing:**  
  Variables can hold **any type of value** and their type can change at runtime.

---

### Example in JavaScript (Dynamic Typing)

```js
let name = "ganja";          // typeof name is "string"
console.log(typeof name);    // Output: string

name = 123;                  // Now name holds a number
console.log(typeof name);    // Output: number
```
![image](https://github.com/user-attachments/assets/bbe09c9e-4eaf-4ee7-9a5e-04caa0519bbd)

dynamic typed: variables can be changes at runtime 

typed of operatior 
![image](https://github.com/user-attachments/assets/a9731706-4de1-4a43-a9e4-aad4a0323972)
for the given data
![image](https://github.com/user-attachments/assets/f591bb71-578c-41e7-a334-8830e54e1630)


# Objects

- Objects are **reference types** in JavaScript.
- Common reference types include:
  - **Objects**
  - **Arrays**
  - **Functions**

---

### Why Use Objects?

- When dealing with **related variables**, we can group them inside an **object**.
- This helps to represent complex data, like a **person** with multiple properties.

---

### Example: Representing a Person

```js
let person = {
  firstName: 'John',
  lastName: 'Doe',
  age: 30
};
```

![image](https://github.com/user-attachments/assets/f55a69a4-7174-4892-aa13-499a4ee2b43c)

![image](https://github.com/user-attachments/assets/adf3514a-902b-4cb8-ae72-6dbf8016a28e)

![image](https://github.com/user-attachments/assets/947f2337-34f8-4dd4-b409-77dae33461db)

![image](https://github.com/user-attachments/assets/1ca8f9fd-5d71-4e89-82d7-2cf0cad034c3)

or 
# Accessing and Changing Object Values

- To **refer to** or **change** a value inside an object, use **dot notation**.

---

### Example:

```js
let person = {
  firstName: 'John',
  lastName: 'Doe'
};

// Access value
console.log(person.firstName);  // Output: John

// Change value
person.firstName = 'Jane';
console.log(person.firstName);  // Output: Jane
```

using bracket notation
![image](https://github.com/user-attachments/assets/e440ee47-9478-4a66-b6cc-b37af0c81446)


# arrays
![image](https://github.com/user-attachments/assets/09bec0d1-d428-4cf0-8bcd-16240145377c)
![image](https://github.com/user-attachments/assets/ff37e113-2301-43f5-8aff-0f2b233dbb8b)

we can access them using index

we can add them using the index
![image](https://github.com/user-attachments/assets/4bdd94af-dfc6-4106-86fd-abf4a9daf075)
![image](https://github.com/user-attachments/assets/3b063ba8-b96a-43cc-9546-0c6687d02386)

in js we can have diff types too in an array 
![image](https://github.com/user-attachments/assets/611c6238-80c6-4358-9c3a-e96e25623159)





type: 
![image](https://github.com/user-attachments/assets/da65a7fc-7da9-4d38-9d7f-204e69b6cd31)

it has no of properties used with dot notation , length...
![image](https://github.com/user-attachments/assets/1ac10ff5-3276-4744-b738-5e69569504d9)

# next is functions 

fundamental building blocks 
perfomrs a task / calculates a val 

![image](https://github.com/user-attachments/assets/846651d5-b306-4ab2-aaf6-3e67b3592a43)
![image](https://github.com/user-attachments/assets/50b77c1c-7a1c-4de9-92c6-67c12bd4c40a)


it can also have inputs too 
![image](https://github.com/user-attachments/assets/6998a470-2027-4bc5-b07d-06df356770ad)
![image](https://github.com/user-attachments/assets/87e9b0d9-fd9a-4151-88df-9734a21db50b)

types of function : 
log function and square function 
![image](https://github.com/user-attachments/assets/8ccfae33-ab53-4043-a281-85d2b9a86c3c)

