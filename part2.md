## NYCDA Backend Exam - Part 2

Given that we have a "customer" resource/model in our web server,

# 1 - How would you design the routes of your server based on REST convention? List them with VERB and /route

app.post('/users/register'      - create user
app.get('/users/show'           - show user data
app.put('/users/:id'            - edit user data
app.delete('/users/delete'      - delete user

# 2 - Which pages would require templates, and how would you name them? List them with /route and template-name.extension

register user:      /views/users/new.pug
edit user:          /views/users/edit.pug
show user data:     /views/users/show.pug

# 3 - What is a database constraint? Name the 3 types of database constraints you have learned.

A constraint for a column in a table in a database. allowNull, unique, foreign key.

# 4 - What is a foreign key? Given that you have a Factory that has many cars and car that belongs to a factory, What would be your foreign key column?

A column in a table that contains the id of a row in another table, to connect the
data in the table to the other table, for example when multiple comments need to be
connected to a single blog post. factoryId in the car table.

# 5 - List all the model lifecycle hooks you have learned from sequelize and explain them briefly if necessary.

Create - create the model / insert data
Read - read data from the model
Update - change/edit data in the model
Destroy - delete the model

# 6 - What is the difference between database-level validations and application-level validations?

In database-level validation data sent from the client is compared to data in the
database, like a username someone types is compared to the username in the database.
In application-level validation data is compared to constraints put to it, like if a password is shorter than 50 characters.

# 7 - Why do we use bcrypt. Write down 3 reasons why we use it if you can.

- bcrypt makes passwords unreadable and undecipherable because it uses hashing,
so it doesn't store the password itself, but compares hashes to decide if the password
is right

- bcrypt is relatively slow in comparing hashes, which also slows the time needed to crack a
password

# 8 - What is a flash message?

A message that can sort of pop up in the page when the user interacts with the page,
like when they put in the wrong password.

# 9 - What is the difference between minifying and obfuscating JavaScript?

Minifying is used to make a file as small as possible but still readable for the
client, for example taking out the white spaces, to make a page work faster.
Obfuscating is used to make a JS file unreadable (for people) to protect its content,
while it also still works in the client (browser), for example by changing variable
names.

# 10 - What are the 3 reasons that makes Gulp a good choice as an asset build library?

- has a large community
- you can write in JavaScript
