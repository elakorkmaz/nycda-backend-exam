## NYCDA Backend Exam
=====================
Explain the questions well!!

### 1- Why do we should include script tags at the very end of an html file, before closing </body>?

So the static content is loaded before the dynamic content. This makes the page
faster to load.

### 2 - What is a middleware?

Middleware is code to modify standard objects in express so you can add functionalities or
change how the objects work out in the webpage.

### 3 - Why do we use express.static() middleware?

To use static files like html and images on the server and provide a path where
express can acces them.

### 4 - What is favicon.ico ?

The icon that is shown when someone bookmarks the site and is shown in the url bar.

### 5 - Why do we use a bodyParser middleware ?

To parse the body of data that is sent by the user on the client side so it can
be 'read' by the server.

### 6 - What is the difference in terms of parsing a data received from a web form with POST or an AJAX POST request?

I don't know.

### 7 - Why do we use methodOverride middleware ?

So you can override the use of 'method' in a form, e.g. use app.delete and app.put instead of app.post

### 8 - What are the differences between sessions and cookies ?

Sessions are created on the server side when someone is using a webpage, like when
they log in, and only last as long as the user is on the webpage.
Cookies are created and stored on the client side and can be modified
by the user, they can be stored infinitely or as long as they have been programmed
to be stored or the user can delete them.

### 9 - Why do we use a session middleware ?

To store data encrypted during a session, for example when a user is logged in. the
middleware also enables you to choose where to store the data, so it provides more
options.

### 10 - Why do we use a build process ?

A build process can be used to optimize files, put them together and make them smaller
so the page can load faster.
