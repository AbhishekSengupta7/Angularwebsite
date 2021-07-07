=======================
Web Application
=======================

The web application is created on the Typescript framework using Angular CLI version 12.0.3. Angular CLI requires node.js as a prerequisite. To setup node.js and angular execute the following commands :  

*sudo apt update*

*sudo apt install nodejs* 

*sudo npm install -g @angular/cli*

Installing dependencies
============================

Navigate to the Energy-predictor folder and execute the following command:

*npm install*

npm install downloads dependencies defined in a package. json file and generates a node_modules folder with the installed modules.

Build
============================

Navigate to the Energy-predictor folder and run the following command to build the application.  

*ng build*

The command builds and bundles the application for deployment.The build artifacts will be stored in the dist/ directory.

Run the Web Application
============================
Navigate to the Energy-predictor folder and run the following command to start the client. 

*ng serve*

The command uses default port number 4200 to run the angular application. And our application URL will be http://localhost:4200. Navigate to this link to check the web application. 

References
============================

https://angular.io/cli
