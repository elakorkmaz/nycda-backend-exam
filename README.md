## NYCDA Backend Exam
=====================
Explain the questions well!!

### 1- Why do we should include script tags at the very end of an html file, before closing </body>?

So the static content is loaded before the dynamic content. This makes the page
faster to load and makes sure it is displayed also when the js is not working properly.

### 2 - What is a middleware?

Middleware is code to modify objects in express, so you can change how it works
out in the webpage.

### 3 - Why do we use express.static() middleware?

To access static files like html and images while using express

### 4 - What is favicon.ico ?

The icon that is shown when someone bookmarks the site and is shown in the url bar.

### 5 - Why do we use a bodyParser middleware ?

To read data posted by the client.

### 6 - What is the difference in terms of parsing a data received from a web form with POST or an AJAX POST request?

With POST data is sent to the database and then the page has to reload or
redirected. With AJAX POST the data is sent while staying on the page.

### 7 - Why do we use methodOverride middleware ?

So you can use app.delete and app.put instead of app.post

### 8 - What are the differences between sessions and cookies ?

Sessions are stored on the server side and cookies on the client side. Cookies
can be saved for a longer time than sessions. Session store strings, cookies store
objects. Sessions are more secure than cookies.

### 9 - Why do we use a session middleware ?

To store data encrypted during a session, for example when a user is logged in.

### 10 - Why do we use a build process ?

To provide a standard, so your code is understandable for others.
