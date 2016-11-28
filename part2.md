Given that we have a "customer" resource/model in our web server,

1 - How would you design the routes of your server based on REST convention? List them with VERB and /route

get /name
get /name/:id
put /name/:id
post /name
delete /name/:id
get /name/new
get /name/:id/edit
get /login
get /logout
get /forget-password



2 - Which pages would require templates, and how would you name them? List them with /route and template-name.extension

pages that will display on the browser.
index, show, edit, new

get /name - index.pug
get /name/:id - show.pug
get /name/new - new.pug
get /name/:id/edit - edit.pug
get /register - register.pug
get /login - login.pug
get /forget-password - forget-password.pug




3 - What is a database constraint? Name the 3 types of database constraints you have learned.
to
require property in a table must follow:

null
unique
primary key
foreign key

4 - What is a foreign key? Given that you have a Factory that has many cars and car that belongs to a factory, What would be your foreign key column?
Is like post and comment.
The post has the primary key and the foreign key are the comments.


5 - List all the model lifecycle hooks you have learned from sequelize and explain them briefly if necessary.

create = create the model
read = read the model
update = change the model
destroy = delete the model

6 - What is the difference between database-level validations and application-level validations?
data base level = constrainds
application-level = validations

7 - Why do we use bcrypt. Write down 3 reasons why we use it if you can.
To hide the original password.
Not easy to hack the password, it will slowdown.


8 - What is a flash message?
a middleware to send errors back to the client
Just like if you typed the wrong password you will get the error message.

9 - What is the difference between minifying and obfuscating JavaScript?
Both files are modified JS files.

minifying is modified to remove all the unnecessary characters in the file. This will make the JS file lighter and it will load faster.

obfuscating is modified to make the JS file difficult to understand and read. People can not copy the source code to their own projects.


10 - What are the 3 reasons that makes Gulp a good choice as an asset build library?
I don't know


I think everyone use the same library for the css/js
You can change the codes of the js/css file from bootstrap
