# newServer

##install nvm

##install node

##install git

##install mongodb
[Install MongoDB Community Edition on Debian](https://docs.mongodb.com/manual/tutorial/install-mongodb-on-debian/)
#####Follow these steps to install MongoDB Community Edition using the apt package manager:

######1-Import the public key used by the package management system
 From a terminal, issue the following command to import the MongoDB public GPG Key from https://www.mongodb.org/static/pgp/server-5.0.asc:
```
wget -qO - https://www.mongodb.org/static/pgp/server-5.0.asc | sudo apt-key add -
```

#####Create a `/etc/apt/sources.list.d/mongodb-org-5.0.list` file for MongoDB.

Create the list file using the command appropriate for your version of Debian:

`echo "deb http://repo.mongodb.org/apt/debian buster/mongodb-org/5.0 main" | sudo tee /etc/apt/sources.list.d/mongodb-org-5.0.list`

#####Reload local package database:

Issue the following command to reload the local package database:

`sudo apt-get update`

#####Install the MongoDB packages:


To install the latest stable version, issue the following

`sudo apt-get install -y mongodb-org`

##Run MongoDB Community Edition
####1-Start MongoDB.
`sudo systemctl start mongod`
####2-Verify that MongoDB has started successfully
`sudo systemctl status mongod`
####3-Begin using MongoDB:
Start a `mongosh` session on the same host machine as the `mongod`. You can run `mongosh` without any command-line options to connect to a `mongod` that is running on your localhost with default port 27017.

`mongosh`


---
