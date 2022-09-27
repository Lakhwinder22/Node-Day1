1. Node.js 

- It is launched on 2014 by Ryan Dahl.
- It is an open-source and cross-platform runtime environment for executing JavaScript code outside a browser.
- NodeJS is not a framework and it’s not a programming language. 
- Node js is the server side of js
- It helps to run js on our OS directly
- We often use Node.js for building back-end services like APIs like Web App or Mobile App. 
- It’s used in production by large companies such as Paypal, Uber, Netflix, Walmart, and so on.

Features of NodeJS: 

- It’s easy to get started and can be used for prototyping and agile development
- It provides fast and highly scalable services
- It uses JavaScript everywhere, so it’s easy for a JavaScript programmer to build back-end services using Node.js
- Source code cleaner and consistent.
- Large ecosystem for open source library.
- It has Asynchronous or Non-blocking nature.

Advantages of NodeJS: Here are the benefits of using Node.js 
 
Easy Scalability: Developers prefer to use Node.js because it is easily scaling the application in both horizontal and vertical directions.

Real-time web apps: If you are building a web app you can also use PHP, and it will take the same amount of time when you use Node.js, But if I am talking about building chat apps or gaming apps Node.js is much more preferable because of faster synchronization. Also, the event loop avoids HTTP overloaded for Node.js development.

Fast Suite: NodeJs runs on the V8 engine developed by Google. Event loop in NodeJs handles all asynchronous operation so NodeJs acts like a fast suite and all the operations can be done quickly like reading or writing in the database, network connection, or file system

Easy to learn and code: NodeJs is easy to learn and code because it uses JavaScript. If you are a front-end developer and have a good grasp of JavaScript you can easily learn and build the application on NodeJS

Application of NodeJS: 

Real-Time Chats,
Complex Single-Page applications,
Real-time collaboration tools,
Streaming apps
JSON APIs based application
--------------------------------------------------------------------------------------------------------------------------
2. What is NPM?

- NPM stands for the node package manager, npm is used for node dependency management. Most of the time, we use npm as a server-side node dependency tool.

1. NPM gets installed with NodeJs installation.
2. NPM uses nested dependencies, so we can use different versions of any module in our code.
- Nested dependencies mean that any dependency is again dependent on another dependency
- npm: It is a package manager for the JavaScript programming language.
- It is the default package manager for the JavaScript runtime environment Node.js.
- Help to manage a project’s dependencies. 
- npm is installed with Node automatically.
- npm: NPM generates a ‘package-lock.json’ file. the package-lock will generate the same node_modules folder for different npm versions.
------------------------------------------------------------------------------------------------------------------------------------------

3. What are the modules in Node.js?

- In Node.js, Modules are the blocks of encapsulated code that communicates with an external application on the basis of their related functionality.
- Modules can be a single file or a collection of multiples files/folders.
- The reason programmers are heavily reliant on modules is because of their re-usability as well as the ability to break down a complex piece of code into manageable chunks.

Modules are of three types:

Core Modules/Internal modules
local Modules/Custom modules
Third-party Modules

1. Core Modules: Node.js has many built-in modules that are part of the platform and comes with Node.js installation. These modules can be loaded into the program by using the require function.
- The require() function will return a JavaScript type depending on what the particular module returns. 
ex:- http	creates an HTTP server in Node.js.

2. Local Modules: Unlike built-in and external modules, local modules are created locally in your Node.js application. Let’s create a simple calculating module that calculates various operations.
Another file can use its exported functionality using the require() function.

3. Third-party modules: Third-party modules are modules that are available online using the Node Package Manager(NPM). These modules can be installed in the project folder or globally. Some of the popular third-party modules are mongoose, express, angular, and react.

Example:

npm install express

------------------------------------------------------------------------------------------------------------------------------------------

4. What is the purpose of the module.exports?

- Module.exports are the instruction that tells Node. js which bits of code (functions, objects, strings, etc.) to “export” from a given file so other files are allowed to access the exported code.
- The module.exports is actually a property of the module object in node.js. module. Exports is the object that is returned to the require() call. By module.exports, we can export functions, objects, and their references from one file and can use them in other files by importing them by require() method.
- easy to maintain and manage the code base in different modules.

------------------------------------------------------------------------------------------------------------------------------------------

5. Difference between default export and named export

-  export objects, functions, variables from the module so they can be used by other programs with the help of the import statements. There are two types of exports. One is Named Exports and other is Default Exports. 

Named Exports: Named exports are useful to export several values. During the import, it is mandatory to use the same name of the corresponding object. 

- Named Exports:-
Named exports allow us to share multiple objects, functions or variables from a single file and were introduced with the release of ES2015.
- Named exports are imported with curly braces in various files and must be imported using the name of the object, function or variable that was exported.

// Exporting individual features
export var name1 = …, name2 = …, …, nameN; // also let, const
 
// Export list
export { name1, name2, …, nameN };
 
//Exporting everything at once
export { object, number, x, y, boolean, string }
 
// Renaming exports
export { variable1 as name1, variable2 as name2, …, nameN };
 
// export features declared earlier
export { myFunction, myVariable };

- Default Exports: Default exports are useful to export only a single object, function, variable. During the import, we can use any name to import. 

- Exports without a default tag are Named exports.
 Exports with the default tag are Default exports. 
- default export:-
Using Named and Default Exports at the same time: It is possible to use Named and Default exports in the same file. It means both will be imported in the same file. Example: javascript.

// file module.js
var x=4;
export default x;
 
// test.js
// while importing x in test.js
import y from './module';
// note that y is used import x instead of
// import x, because x was default export
console.log(y);       
// output will be 4

------------------------------------------------------------------------------------------------------------------------------------------

6. How do you import any module in Node.js

- Importing functions or modules enhances the reusability of code. 
- Importing a Module: We need to import the module to use the functions defined in the imported module in another file. The result returned by require() is stored in a variable which is used to invoke the functions using the dot notation.

- const f = require('./func')
------------------------------------------------------------------------------------------------------------------------------------------