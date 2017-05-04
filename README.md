# customer-version
I have put here some code for the app.

Now this has some functionnalities, it has some limits

## Adding a database
- Open MySQL interface(e.g PhpMyAdmin)
- Import the file located in Database/ folder.
- You can choose either customer.sql or customer-without-data.sql
  The second file do not have data exported from my database as the first one.

## Connecting the application to the database
- Go to the folder WebApplication/app/var/db.php
- Edit the file to provide the host name, the username, the MySQL user password and the database name
- Save and close the file

## Adding a user: a customer or an agent
- To add users to the database, you should add in MySQL 
  Example: To add an customer, first, add a User,then add a Customer. To add an agent, add a User, then an agent.

## Launching the webSocket Server
- This server uses the Ratchet library for WebSocket in PHP. This library uses Composer and Symphony. They should be added. I currently use Ubuntu and AMPPS and I have installed these libraries. If you use Windows and if they are not yet installed in your PHP server, please add them.
- After adding these libraries, move to folder WebSocketServer, copy it to any other folder in which you have rights to execute the file.
- After having the folder, well placed, go to bin/ in this folder and run the file webSocket.php in the CLI by the command
  php webSocket.php
  
## Running the whole project
- After adding these, you can create a domain or subdomain that directly open www/ folder for some security. In this way, the classes are safe in app/.
- Login with the created credentials
- You can login with the agent username and password or the customer's.
- The tickets are created from the username account.

## Acknowlegdement
The app do not support many functionnalities. I just designed it to show my level in web programming.
