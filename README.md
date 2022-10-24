# Games Hub

Games Hub is a full stack JavaScript application with an Express server and MongoDB database.

## Getting Started

These instructions will get the project up and running on your local machine for development purposes.

### Installing

Install dependencies in both the client and the server folders:

```
cd client
npm install

cd server
npm install
```

Seed the database.  Within the server folder:

```
npm run seeds
```

Run express (leave running in a terminal window).  Within the server folder:

```
npm run server:dev
```

Run React environment (leave running in a terminal window).  Within client folder:

```
npm start
```

### Using

The application is running on port 3000 so visit http://localhost:3000/.




<!-- Task
Draw a diagram showing the dataflow through the application starting with a form submission, ending with the re-rendering of the page. This will involve a multi-direction data-flow with the client posting data to the server and the server sending data back to the client with the response. Detail the client, server and database in the diagram and include the names of the files involved in the process. -->

Questions
<!-- 1 What is responsible for defining the routes of the games resource? -->
    The create_router.js file

<!-- 2 What do you notice about the folder structure? Whats the client responsible for? Whats the server responsible for? -->
    Client is responsible for form handling and rendering web pages

<!-- 3 What are the the responsibilities of server.js? -->
    For connecting the database/Api to the client files

<!-- 4 What are the responsibilities of the gamesRouter? -->
    

<!-- 5 What process does the the client (front-end) use to communicate with the server? -->
    Vue CLI

<!-- 6 What optional second argument does the fetch method take? And what is it used for in this application? Hint: See Using Fetch on the MDN docs -->
    Error Catching 

<!-- 7 Which of the games API routes does the front-end application consume (i.e. make requests to)? -->
 .get('/') .post('/')

<!-- 8 What are we using the MongoDB Driver for? -->
 For storing non relationship data

Extension
<!-- Why do we need to use ObjectId from the MongoDB driver? -->
    To select a single object for things such as updating or deleting

<!-- Add to your diagram the dataflow for removing a game. -->

