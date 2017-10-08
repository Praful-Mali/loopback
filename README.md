# My Application

Install

Assuming you have already installed Node...

Step-1

Install the LoopBack CLI tool....
$ npm install -g loopback-cli

Step- 2

$ lb
? What's the name of your application? hello-world
? Enter name of the directory to contain the project: hello-world

? Which version of LoopBack would you like to use? 3.x (current)
? What kind of application do you have in mind? hello-world (A project containing a controller,
including a single vanilla Message and a single remote method)
...
I'm all done. Running npm install for you to install the required dependencies.
If this fails, try running the command yourself.
... 

Step-3

Create models
$ lb model

The generator guides you through creating your model. 
Enter the values highlighted in green. 
To accept the default, just press Enter.
[?] Enter the model name: register
[?] Select the data-source to attach person to: db (mongodb)
[?] Select model`s base class (PersistedModel)
[?] Expose person via the REST API? Yes
[?] Custom plural form (used to build REST URL): register
[?] Common model or server only? common
Let's add some person properties now.

Define a firstname property for the person model
Enter an empty property name when done.
[?] Property name: name

Hit Enter to accept the default string type:
[?] Property type: (Use arrow keys)
❯ string
  number
  boolean
  object
  array
  date
  buffer
  geopoint
  any
  (other)


Make the property required.
[?] Required? (y/N) y


Repeat these steps for lastname property.

Press Enter when prompted for a property name to finish up and create the model.


Run the application

Run as you would any Node application.
$ node .
Browse your REST API at http://0.0.0.0:3000/explorer
Web server listening at: http://0.0.0.0:3000/


Connect Mongodb Database

Install the LoopBack MongoDB connector

Step - 1
npm install --save loopback-connector-mongodb

Step - 2
lb datasource datasoruceName

