# Track-My-Reps
An exercise app that tracks user's fitness reps based on user's input.
This app is created using MongoDB, Express, React, and Node.js (MERN) following REST API principle. Currently it is run on a local server using MongoDB connect string to access the database. 
User can enter the exercise along with any additional parameter at a specified date. User can 
also modify existing exercises, or delete it altogether. 

```
08/10/2022 - Add backend API (express, mongoDB, mongoose)

08/17/2022 - Add frontend API (react, HTML, CSS)
```

**NOTE**: You need to install Node.js and npm package to run this program. To get started, check out https://nodejs.org/en/ and download the most current version of Node.js (this program uses version 16.17.0) for your operating system. I will also assume that you already have git installed. If not, check out https://git-scm.com/book/en/v2/Getting-Started-Installing-Git. You will also need to register an account and create a free cluster on mongoDB in order to host your own database. Check out https://www.mongodb.com/cloud/atlas/register

First, clone this repository to your local machine. From the repository, click on Code and copy the HTTPS link.

![Git Clone](https://github.com/dangja92/Track-My-Reps/blob/assets/git_clone.jpg?raw=true)

On your git terminal, change to your desire directory where you would like to clone this app via the following command:
```
cd /my-preferred-directory
```
Then, enter this command to clone the repository:
```
git clone <HTTPS link that you copied earlier>
```

Let's get your mongoDB cluster set up. After you have created an account with mongoDB, you can create a free server by clicking on the 
**Shared** tab. You can choose whichever cloud provider and region you want based on your location. Once everything is set, click **Create Cluster**

![Create MongoDB Cluster](https://github.com/dangja92/Track-My-Reps/blob/assets/mongoDB.jpg?raw=true)

**How to connect:** 
	i.   Create a user account  for this cluster with username and password. Click Create User. 
	ii.  View the User lower on the screen, then choose where to connect from: 
		1.   Our localhost will talk to the DB on Atlas server. We must whitelist My Local Environment. Add your IP address in the My Current IP Address field. 
		2.   View it lower in the screen. 
		3.   Finish and Close to view the Congrats message
		4.   Click **Go to Databases** to view your new Project 0 with Database Cluster 0.

To connect your mongoDB cluster to your backend API, you need to grab the connect string. At your cluster homepage, click **Connect**, then do the following:

![Connect String](https://github.com/dangja92/Track-My-Reps/blob/assets/mongoDB_connect.jpg?raw=true)

Once you've copied your connect string, navigate to the directory where you've cloned this respository. Doubble click on **exercise-tracker-backend**. Find the **.env** file and edit it by pasting your connect string to **MONGODB_CONNECT_STRING**

![ENV File](https://github.com/dangja92/Track-My-Reps/blob/assets/add_connect_string.jpg?raw=true)

Now your mongoDB cluster should be set up for this app.

----------------------------------------------------------------------------------------------------------------------------------------


