# Validation - Exercise #1 - Forms with template strings

In this exercise we are going to build a UI form. We will use this in the following series of exercises to send data to our API. Later on we will validate the sent data step-by-step.

## Build a registration form

* Setup a file server.js
* Install express
    * If `npm i express` does not produce you a node_modules folder: Do `npm init -y` beforehand and install express once more 
* Setup an express app
    * Use the express snippets by typing e4- into your code file and hit tab.
    * Select the entry e4-example-helloworld from the list
    * Now the "port" is automatically selected in the editor so you can replace it
        * Type in 3000
        * Hit ESC on you keyboard
    * You now should have an express app ready to go!
* Setup an middleware for processing incoming form data
    app.use(...)
* Setup a GET route "/register"
    * Build up a form template string and store it in a variable 
        => `const strForm = ...`
    * Place an H1 tag above the form with title "Register"
    * Setup an HTML form
        * use action="/register" and set POST as send method on the form
    * Provide four input fields: 
        * Email
        * Password
        * Use input type "text" for the email and type "password" for the password field
    * Send back the form string with res.send
    * Start the express app using nodemon
    * Test if your form is reachable in the browser
    
* Setup a POST route /register
    => this is the route that will receive the form data
    * Console log the sent form data here
    * For now: Just send the received form data back to the client as a response using res.send

* Testing
    * Call your /register form in the browser and sent data
    * Check your nodemon console if you correctly received the sent data in your post route. It should get printed by your console.log statement

