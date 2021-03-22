# Tasks-backend


## The project
***
The project is a task Api that serves and saves data from a database Postgresql.

## Running
***
For the project to work it is necessary that first inside the folder run the command below, to install all dependencies:

 ```
 npm install
 ```
 Then it is necessary to modify the file **env_file** to **. env**, and put a value in **authSecret**. Then it is necessary to modify the file ** knexfile.js ** by exchanging the data referring to the local database.

So after that inside the folder to start the project it is necessary to run the following command:
 ```
 node index.js
 ```
 ## Routes
 ***

 **Signin:** This route is of the post type and is indexed by the url **/signin**, the body passes the email and password, and authenticates the user.

  **Signup:** This route is of the post type and is indexed by the url **/signup**, the email, name and password are passed through the body, and thus the user data is saved.

 **Save:** This route is of the post type and is indexed by the url **/tasks**, it is passed through the body of the request, parameters such as **user.id**, and **tasks** where it contains the data of the taks.

 **Get Tasks:** This route is of the type get and is indexed by the url **/tasks**, the date is passed or not via query.date, and the answer will be from the taks until that certain date in case there is date will be the current fia.

 **Delete Tasks:** This route is of the delete type and is indexed by the url **/tasks/:id**, the task id to be deleted is passed.

 **Toggle Tasks:** This route is of the put type and indexed by the url **/tasks/:id/toggle**, the id of the task that you want to alternate its completion state is passed.
 