## NYCDA Backend Exam

Explain the answers well!!

### 1- Why should we include script tags at the very end of an html file, before closing  ```</body>```?
We want the page to load all the content before JavaScript, so that all content is loaded before interaction takes place, and the JS functions run after as it is designed to. This also means the static content will load faster and give the user a better experience.


So the static content is loaded before the dynamic content. This makes the page
faster to load.

### 2 - What is a middleware?
Middleware, in the context of node.js/express server are pieces of code/ a function that act in between the server and client. It can execute code, make changes to the request and response object, end the request-response cycle, call the next middleware function in the stack. Middleware generally executes before your route handlers, and it follows a chain via the next(). If you forget to run next() in your custom middleware, the request will never reach your route handler thus the server will hang, without giving the response on time.

Middleware is code to modify standard objects in express so you can add functionalities or
change how the objects work out in the webpage.

### 3 - Why do we use express.static() middleware?
It lets us serve static files over http. Convention is to use ```/public``` as our publicly accessible static-asset space.

To use static files like html and images on the server and provide a path where
express can acces them.

### 4 - What is favicon.ico ?
Small icon at the left of the URL or on the tab, usually the company logo of the website. Its displayed next to the url and in the bookmarks. Mainly for website branding.

The icon that is shown when someone bookmarks the site and is shown in the url bar.

### 5 - Why do we use a bodyParser middleware ?
BodyParser extracts the entire body portion of an incoming HTTP request stream and exposes it on req.body

<<<<<<< HEAD
To parse the body of data that is sent by the user on the client side so it can
be 'read' by the server.

### 6 - What is the difference in terms of parsing a data received from a web form with POST or an AJAX POST request?
=======
### 6 - What is the difference between parsing a data received from a web form with POST and an AJAX POST request?
<<<<<<< HEAD
>>>>>>> 80d83206a180f1ae39386af476c8c9ff4b8addb1

I don't know.
=======
both request would hit the same route and run the same code. The difference is the body parsing. Web forms serialize the data as formurlencoded format while AJAX POST request is a stringified JSON. Also both request would expect different type of responses, json request could receive a json response while web form requests generally receive redirect as a response and a status code.
>>>>>>> c949bffaf101f8989f7569cdd7ec4090f2180609

### 7 - Why do we use methodOverride middleware ?
web forms dont support PUT and DELETE request. MethodOverride is a hack that turns POST requests to PUT or DELETE if the webform has ```<input type="hidden" name="_method" value={{HTTP METHOD}}>``` field

So you can override the use of 'method' in a form, e.g. use app.delete and app.put instead of app.post

### 8 - What are the differences between sessions and cookies ?
Sessions is stored on the server side, cookies are on the client side. Cookies store primitive data types like strings, integers and boolean while sessions can store objects. Sessions is a more secure way of saving data. Cookies can be saved for a longer period of time and you can expire them both.

Sessions are created on the server side when someone is using a webpage, like when
they log in, and only last as long as the user is on the webpage.
Cookies are created and stored on the client side and can be modified
by the user, they can be stored infinitely or as long as they have been programmed
to be stored or the user can delete them.

### 9 - Why do we use a session middleware ?
HTTP is request/responses normally are stateless it is hard to tell the difference between two random requests. Session middleware lets us access the persistent session across all our route handlers, under req.session. Middleware uses a cookie key on the clients browser. Cookie stores a session reference, that is how the server/middleware read(cookies are sent to the server in each request) and find the relevant session. req.session is an object accessible throughout your route handlers.

To store data encrypted during a session, for example when a user is logged in. the
middleware also enables you to choose where to store the data, so it provides more
options.

### 10 - Why do we use a build process ?
<<<<<<< HEAD

A build process can be used to optimize files, put them together and make them smaller
so the page can load faster.
=======
Build processes allow task automation. You can optimize your frontend assets(css and js) and do file operations on the fly for them like minification or obfuscation with build tasks/processes.
>>>>>>> c949bffaf101f8989f7569cdd7ec4090f2180609
