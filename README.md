#Linux Server Configuration Project

##Introduction
The purpose of this project is to demonstrate the ability to configure a linux server and to deploy and serve an existing Python web app.

##Requirements
To view the app being hosted, the only requirements are a modern browser, internet connnection, and the IP address of the server.

For grading and inspecting the server, a shell and the ability to remotely login via ssh, along with the login info are required.

##App Functionality

+ Root page displays a list of movie categories and movie names
+ Anyone can navigate to specific movie pages to see their description
+ Users are able to create new movies for the database, and edit/delete movies that they have created
+ Non-registered users, or users that don't have permission to edit/delete movies do not see links to create/update/delete
+ Additionally, the backend protects these operations from attempts to access them from outside of the browser

##Viewing Information
+ IP Address: 18.219.97.108
+ Domain Name Address: http://ec2-18-219-97-108.us-east-2.compute.amazonaws.com

**IMPORTANT**: *in order for the login functionality to work, you will need to access the website via the Domain Name Address*

##Software Installed
+ Python
  + sqlalchemy
  + flask
  + oauth2client
  + request
  + Flask-Login
+ pip
+ Apache
+ Postgres
+ libapache2-mod-wsgi

##Summary of Configurations
+ Disabled remote root login
+ grader user created and given superuser priveleges
+ Disabled password based login
+ Created ssh-keys for remote login
+ Configured UFW to only allow ports 80, 2200, 123
+ Configured ssh to use port 2200
+ Postgres configured to host database
+ Apache configured to serve app on port 80
