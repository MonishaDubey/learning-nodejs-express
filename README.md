# learning-nodejs-express

Starting with Node.js , there are many useful tools that you can use called packages and the system npm (Node Package Manager) allows users to share or download packages. Express is one of them.

Before working on it, we need to check versions of following as :-
                                                   
                                                   node --version
                                                   npm --version
# Moving with working on project:-

Express is a framework for nodejs that provides efficient tools for developing webapps.

Run these commands :- 
                                                   
                                                   mkdir file-name
                                                   npm init(initializing the project with file downloading eg. package.json)
                                                   npm install express --save (downloading express dependencies, modules and what all needed for project)
# Creating An Express App instance 

Wrting these code in app.js file after creating it:-
                                                    
                                                    const express  = require('express'); //Importing package
                                                    const app = express(); // Creating instance
                                                     

# Routing :-  Deteremining how app responds  to a request to a particular URL is called Routing. 
 Middleware is attached on an app instance. Configuration keys can be set on this app instance. 

                                                    app.set('secret key','12345');
# Creating HTTP server in Express
                                                    app.listen(3000, function(){
                                                    console.log('HTTP Server started successfully')
                                                    });                   //Any number port you want to run as localhost .
Now we also need endpoints to connect to our express web server for clients trying to get informations from it. Clients can use those endpoints to connect to get or provide information from it. Routes or Endpoints are URI(Uniform Resource Identifier)  
                                                    
                                                    Routes = HTTP_VERB(GET,POST,UPDATE,DELETE,PUT) + RESOURCE_ENDPOINT 

Each route can handle a request with a function, known as a route handler, that has req (request) and res (response) as parameters. These two parameters will hold information about the request and response. We can specify which view file to show on the browser using the res.render('html file') function.
 
                                                    // Add the route for the top page
                                                    app.get('/top',(req,res) =>{
                                                    res.render('top.ejs');
                                                    });
# Applying CSS
With Express, We need to specify where we have placed our CSS files and image files.

                                                    app.use(express.static('images'));  
We'll add a CSS file to the public folder. To load the CSS, we need to specify the path of the CSS file relative to the public folder.

# Get endpoint / Route in express
                                                    
                                                    app.get();
Installing Nodemon command :-                       npm install -g nodemon


