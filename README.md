# chatbot.api.js ![status](https://github.com/leandro-hl/chatbot.api.js/actions/workflows/node.js.yml/badge.svg)

## ENVIRONMENT
* Install SQL Server Express (And Management Studio if you want to make your own queries). https://www.microsoft.com/en-us/sql-server/sql-server-downloads
* Install SQL Management Studio in order to run database script
* Create bot SQL user and login
* Once installed, make sure TCP/IP connection (port 1433) is enabled in your database 
  * (SQLManager{VERSION}) -> Network configuration -> Protocols -> enable
  * On IP Addresses tab set tcp port
* npm i to install dependencies
* Ask for environment file .env

### ------ To Generate SQL Databse Schema -------
* Open SQL Management Studio, select "Query" in the toolbar and check "SQLCMD Mode".
* Press "New Query"
* Paste and execute the Database Script

### ------ To Start API ------
* npm run dev
* F5 to attach vs code debugger to nodemon process 9230
* port 3000

### ------ To Test the API -----
* Open Postman
* Make a POST request to http://localhost:3000 + timeat / timepopularity
* Set Body RAW JSON with content like { "Timezone": "Vancouver" }
