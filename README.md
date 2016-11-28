## NYCDA Backend Exam
=====================
Explain the questions well!!

### 1- Why do we should include script tags at the very end of an html file, before closing </body>?
to load all the html/css files first and then the JS files.
the website will load faster


### 2 - What is a middleware?
is a function that have access for request object and response object


### 3 - Why do we use express.static() middleware?
In order to use css and js files in a public directory within an express app

lets us serve static files over http

### 4 - What is favicon.ico ?
a logo in the browser url bar.
Company can set their logo as a favicon.


### 5 - Why do we use a bodyParser middleware ?
bodyParser will extract the whole body portion of incoming request.

and then it exposes the data under req.body throughout our route handlers


### 6 - What is the difference in terms of parsing a data received from a web form with POST or an AJAX POST request?
Web form with post it will reload the page.
and Ajax post request it will stay in the same page.

 both request would hit the same route and run the same code. The difference is the body parsing. Web forms serialize the data as formurlencoded format while AJAX POST request is a stringified JSON
 so only the parsing is perhaps the http response is the different, js execution is the same
bodyParser lets us parse the body part of an HTTP request and exposes it under req.body inside the route handlers

### 7 - Why do we use methodOverride middleware ?
To delete the content

web forms dont support PUT and DELETE request. MethodOverride is a hack that turns POST requests to PUT or DELETE if the webform has <input type="hidden" name="_method" value={{HTTP METHOD}}> field


### 8 - What are the differences between sessions and cookies ?
sessions will store the data on the server and cookies will saved the data on the visitor browser.
Sessions is more secure.

### 9 - Why do we use a session middleware ?
I don't know.
But I think it will save the data during the request object and response object.


middleware lets us access the persistent session across all our route handlers, under req.session. Middleware also uses a cookie on the clients browser. Cookie stores a session reference, that is how the server/middleware can find the relevant session.

### 10 - Why do we use a build process ?
build process of each line step by step of the life cycle

I don't know

Build process(like gulp) optimizes our frontend css/js and let us do file operations on them
