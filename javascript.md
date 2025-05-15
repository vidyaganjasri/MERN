js: 
programmign language

with js can work as 
front-end
back-end
full stack dev


initially used in browsers to work with front-end 
thse days web/mobile apps, real-time networking application(likc chats),cmd line tools,
games

where does it run 
intially only on browsers, it has javascript engine: firefox: spiderMonkey, chrome:v8
2009 
Ryan v8 embedded in c++: Node 

with this we can run jscode outside of a browser in node 

ecmascript: specification 
javascript: whocih confimrs specificiation 


# Commands 
go to chrome 
click on inspect and select console which is js console 

![image](https://github.com/user-attachments/assets/77446bc8-3e9e-49b3-9894-a4cb18b6acd2)

![image](https://github.com/user-attachments/assets/56aecb99-22f7-4949-bf79-9dfe0e0ff5fd)


Setting up dev env: 
code editors: vscode, sublime text 

set your envir as in the image
![image](https://github.com/user-attachments/assets/03492717-a1c3-450f-926b-55f2ea5cc7a0)

NOw there are two places where you can include your code 
in the head section 
or in the body sectoin 
the best practice at the end of body sectionafter every elements
as the browser process this file top to bottom so it will be able to render html 
the code in b/w script needs to talk to the body elements so they should be declared first 

console.log("Hello World");
writing this in the script file
all the statements should be terminated by semicolon 
"Hello World" is a strign 

in js : // this represents a comment, ignored by js, not executed but for documentation
more like why are doing this instead of what it does 


to look at the output 
![image](https://github.com/user-attachments/assets/d83592e3-66b3-4f50-8d29-c21fae8b3d51)
go to the webpage
inspect go to console 
or alternatively
alt+ctrl+i kk this is not working
![image](https://github.com/user-attachments/assets/8edc4321-6307-49c2-a252-a19ff896ef87)


Seperation of concerns to seperate html and js file 
still works
![image](https://github.com/user-attachments/assets/8db75296-483e-421d-9217-b28de305cf94)
![image](https://github.com/user-attachments/assets/28a0190d-26a7-435e-b7e4-40024d2a44c0)


![image](https://github.com/user-attachments/assets/d77e22d4-7ade-44a1-9709-e5046e6da8e9)



so far we ran js in browser
how to do it on node js 
go to the directory nad type node file.js
![image](https://github.com/user-attachments/assets/0848165a-d86c-4ef6-92ce-1515cf2259f6)


even in our vscode itself, insetead of explicity doing it in cmd 
![image](https://github.com/user-attachments/assets/7cae88ec-366d-411a-9917-a0353fdf0994)


# variables 
var to store data temp in computer memory 
a var is box, what is inside is data, label on box is name of var 

to declare a var: 
let name; 
so by default var values are undefined 
![image](https://github.com/user-attachments/assets/74c2365b-0e34-4810-9788-445ec7ceca21)


rules: 
shouldn't be a reserved keyword, let, if ,var, else
should be meaningful
cannot start with a numb
cannot contain space or hypen 
should follow camel notation : firstName
are casesensitive

types of decleartion : 
let firstName="ganja", lastName ="vidya";

best Practice:
let firstName='ganja';
let lastName='vidya';

if we want our var to be fixed use const instead of let
![image](https://github.com/user-attachments/assets/89646836-ee9b-4672-9b77-2deb0eec4926)



types of data types: 
primitive and reference types

primitive: 
strings, numbers, boolea, undefined, null
![image](https://github.com/user-attachments/assets/f2d249cb-d2f7-40b0-aa98-c6be0d31eda1)

js is dynamic language 

two types: 
static : variables are fixed and cannot be changed in the future 


for the same above code if we run in the browser, initially the typeof name would be string 
but if we change the value of name which is usually allowed in the dynamically types lange
and again validate the type it would return number 
![image](https://github.com/user-attachments/assets/bbe09c9e-4eaf-4ee7-9a5e-04caa0519bbd)

dynamic typed: variables can be changes at runtime 

typed of operatior 
![image](https://github.com/user-attachments/assets/a9731706-4de1-4a43-a9e4-aad4a0323972)
for the given data
![image](https://github.com/user-attachments/assets/f591bb71-578c-41e7-a334-8830e54e1630)


# objects
reference types 
objects, 
arrays
functions

when dealing with relateble var we can put it inside an object
reprsentation of person 
![image](https://github.com/user-attachments/assets/f55a69a4-7174-4892-aa13-499a4ee2b43c)

![image](https://github.com/user-attachments/assets/adf3514a-902b-4cb8-ae72-6dbf8016a28e)

![image](https://github.com/user-attachments/assets/947f2337-34f8-4dd4-b409-77dae33461db)

to change/refer the value we use dot notation 
![image](https://github.com/user-attachments/assets/1ca8f9fd-5d71-4e89-82d7-2cf0cad034c3)

or 


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


