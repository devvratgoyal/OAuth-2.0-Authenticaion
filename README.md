# JWT, Web Server and User Agent OAuth flow in Salesforce using Node.js

[![Youtube demo Video](https://img.youtube.com/vi/Iez9xdKbeuk/0.jpg)](https://www.youtube.com/watch?v=Iez9xdKbeuk)

Step 1 : Download and install node.js from https://nodejs.org/en/download/ 
Windows Installer (.msi)

Step 2 : Download /clone the repository from git and extract it to a folder. (Assuming Node.js already installed on system)

Step 3 : Create a ssl certificate or reuse same certificate uploaded in this repository. Refer this post to learn how to create ssl certificate using openssl

Step 4 : Create Connected App in your Salesforce instance with callback URL - https://localhost:8081/oauthcallback.html. Make sure to upload server.crt as a digital certificate in connected app. You can use your own certificate as well.

Step 5 : Copy consumer key & secret created in connected app and update jwt_consumer_key and client_secret variable defined in Server.js file.

Step 6 : Run node.js command prompt and go to the directory where the code was downloaded and 
run npm install command. It will download all the required node modules. Then run npm start, or nodemon Server.js (if installed previously) it will start the server

Step 7 : Navigate to https://localhost:8081/ in your browser and you would see option for all 3 Auth flow - User Agent, Web Server and JWT