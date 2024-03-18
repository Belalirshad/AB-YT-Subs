# AlmaBetter Backend Project

## Get_Youtube_Subscribers

This is a simple backend project that contains a RESTful API for getting information about YouTube channel subscribers. The project is developed with Node.js and Express, and the database used for managing the subscriber data is MongoDB. The subscriber's data consists of fields such as their ID, Names, Subscribed Channels, and Subscription Date.

The API has several endpoints that let users get data in JSON format, such as an endpoint that returns a list of all subscribers, an endpoint that returns a list of names and subscribed channels for each subscriber, and an endpoint that returns information about a subscriber based on their ID.

Web Deployment : https://ab-yt-subs.onrender.com/

## API Endpoints

1. **"/ "** -> This default route will render the "index.html file" when the app launches. 

  ![Main](https://github.com/Belalirshad/AB-YT-Subs/assets/101103105/86613045-8cf3-4db9-b88f-d8be44699c97)

2. **"https://ab-yt-subs.onrender.com/api-docs#/"** -> This route for Swagger Docs.
   
  ![Swagger](https://github.com/Belalirshad/AB-YT-Subs/assets/101103105/25edd61d-0082-4b19-9237-9e79d251fda1)

3. **"/subscribers "** -> This endpoint returns an array of all subscribers in the database. https://ab-yt-subs.onrender.com/subscribers/

  ![Subs](https://github.com/Belalirshad/AB-YT-Subs/assets/101103105/fc48f616-a811-49b1-987f-20a2d636a6f4)

4. **"/subscribers/names "** -> This endpoint returns an array of subscribers with only two fields, their name and subscribed channel. https://ab-yt-subs.onrender.com/subscribers/name
   
  ![Subs_names](https://github.com/Belalirshad/AB-YT-Subs/assets/101103105/2162b52f-e1ed-4930-975f-84821702853d)

5. **"/subscribers/:id "** -> This returns the details of subscriber whose Id is provided in endpoint. https://ab-yt-subs.onrender.com/subscribers/65f485ad87f64a503e4cbba1

  ![Id](https://github.com/Belalirshad/AB-YT-Subs/assets/101103105/c53c4db8-0044-4e4c-8707-c166439da228)
  
## Application Folder Structure

1. [src/app.js] -> For handling requests and responses.

2. [../index.js] -> To connect and start the server.

3. [src/createDatabase.js] -> To create database on MongoDB.

4. [src/data.js] -> Data that has to be connnected to a database.

5. [src/models/subscribers.js] -> For the schema.
   
6. [src/index.html] -> The home page for the application.

```
├── src/
│   ├── app.js
│   ├── createDatabase.js
│   ├── data.js
│   ├── index.html
│   └── models/
│       ├── subscribers.js
├── index.js
├── {} package-lock.json
└── {}package.json
```

## Installation

You'll need to have **Node.js** and **MongoDB** installed on your computer in order to begin working on the project.

Once installed, Clone this repository to your **local** machine.

Install the required dependencies as mentioned below by using **npm install <packageName>**.

Start the server by **node index.js**

## Dependencies

Following dependencie are needed to run this application:

1. express

2. mongoose

3. nodemon

## Team Memebers

- Belal Irshad
- Zainab Faiqua
