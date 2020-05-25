# Demp
This is the demo website for a landing page of a job site with multilevel login

First You go to the main page(index.html).There you can register yourself .Basically what this does is: if the login button is clicked, the login() function is called which logs the user in. Notice that when the user is logged in, it also does a check: if the user is admin, it redirects them to the admin/home.php page. If however, it is just a normal user, he/she is redirected to the index.html page.
The admin can make a user as a user or admin also.
Now you might say, if only an admin can create another admin, then who creates the first admin. Well to create the first admin, you can create a normal user using the registration form, then use any mysql client like phpmyadmin or the mysql command prompt and change the user_type to admin. That way you will be able to log in as admin and create other admins.

As simple as that, we are done with building a system that manages normal users alongside admin users. 

I have created a database using phpmyadmin :-
 created a database called multi_login. In multi_login database, created a table called users with the following fields:

id - int(10)
username - varchar(100)
email - varchar(100)
user_type - varchar(100)
password - varchar(100)
