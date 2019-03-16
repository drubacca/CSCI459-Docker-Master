# Choice of Database Management System

NodeJS/Express/Angular/Mongodb

# Status: accepted

# Context: 

Node.js (also known as Node) is an open source development platform for creating and executing JavaScript code server-side. Node.js is used to run servers that are linked to the javascript code that may serve many purposes. Node.js is intended to run on a dedicated HTTP server and to employ a single thread with one process at a time. Node.js applications are event-based and run asynchronously.

Express is a web application framework for Node.js that allows you to spin up robust APIs and web servers in a much easier and cleaner way. It is a lightweight package that does not obscure the core Node.js features. The specific type of server being run is a Basic Express Server in Node.js, which was created by Michael Auderer. The express app is used in this project as a web app that provides the framework for node. It runs servers in a much cleaner and easier way thus allowing fluidy while working.

Mongoose is a node dependency that makes it very easy to add CRUD (Create Read Update Delete) features that interact with MongoDB. It is very useful for Users to have access to CRUD features because it gives the User controls over the program. Even though the User doesn't have access to the server, they have to ability to add more data, remove, data, and see the data that is currently there while it changes to display their contribution.

# Decision:

The node.js server and basic express server are vital pieces to the MEAN-stack because they allow the developer to create/maintain a RESTful API quickly and without much strain. They bridge the gap between client and management system allowing an API that uses HTTP requests to GET, PUT, POST and DELETE data. The server however does not emphasive ACID properties (which allow the server to guarentee validity even in the event of errors or unlucky events (such as power failures or corrupted hardware)). Node.js/Express/Angular/Mongoose do not need to support ACID properties because the application is event-based and runs asynchronously.

# Consequences: 

It can be difficult to bridge the understanding between Node.js, Express, and Mongoose. It took me awhile to understand and even with source code provided from GitHub it was hard to make sense of.