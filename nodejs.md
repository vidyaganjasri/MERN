node js is open source and cross platform runtim env 
exeting js code out of browser

often used to build backend services
API, power client application , web app, mobile app
![image](https://github.com/user-attachments/assets/b32e48e8-bed6-4fec-a5e2-1581c8ef9133)
need servuces suttubg on serverc, cloud, to store data, push notification 
highly scalable, data intesive and real time app

there are other tools, what's so special 
it;s easy to get started and agile develop
spuerfast and highly sclable, 
uber, paypal, netflix, etc
it uses javascript 
cleaner and more consistent since js in both front'end and backend 
has largest ecosystem of open source lib 

runtime env for js 
before node we use js to run inside broweser
js code - js engine - machine code 

chorome - v8, this is the fast engiene out there
mozialla - spidermonkey

node is runtime env for js code 
plus additional modules not avaliable in browser, work with firesystem etc 

node is not a programming language! it is not a framweork 
it is a runtiem env for executing js code 

how it works: 

highly scalable 
bc non blocking asynchronous nature 
ex: a res , a waiter comes to ur table and gives it to kitchen, they go to another table, while kitechen prepares for the first table

waiter is like a therad, a single thread is used to handles multiple request


blocking synchrnous:
a waiter si alloacated to u, they wait for the chef to prepare the meal completely, will not go to another table until the food is done
ex: asp.net

when a request, a theread is handle the request, when the database is executing the query, so the thread waits, so a new thread serves another query, but threadsa are limited, so they have to wait 
this is limitation there has to do extra hardwork 
but nodes asyn it's not the case, the single thread is used to handle multiple request, when the database is done exeuting it will put it in event queue, which is handled by node, hence makes it ideal, for i/o intensive and real tiemapps, not too much hardware required, 
not use for cpu-intensive apps as lot of operations should be done by cpu, as it will be kept waiting 

how to install node and real time applications 

first run 
create an app.js
and write the following code 
![image](https://github.com/user-attachments/assets/1e83532e-5c95-4e64-8891-4e055f3300a5)
inthe cmd 
run node app.js to see the output 

node module system 






