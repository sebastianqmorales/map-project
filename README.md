### General Application Information

This app was created by a instructor on the Udemy course "The Complete JavaScript Course 2022: From Zero to Expert!" by [Jonas Schmedtmann](https://www.udemy.com/user/jonasschmedtmann/). I worked on this course to help me get a structured understanding of JS and basic CS data structures. I would recommend this course to anyone wanting to learn JS or want a refresher on some basic concepts or ES6 features. This course is strucutred like a college class and is very well done with challenges, homework and great projects, this being one of them.

### Flow Chart

From this flow chart we understand how the user is going to access our application and what technical processes will be required to create these features. This is the starting point of the application architecture.

![flow chart](/pics/Mapty-flowchart.png)

### General Architecture

![final architecture chart](/pics/Mapty-architecture-final.png)

The class App is the entry point to the application, it runs several constructor methods to start crucial app features like geolocation and local storage. The app initalizes the workout class by creating a workout object that contains latitude, longitude and workout type. This object gets passed into the Running or Cycling class.

The Workout class is the parent class of the Cycling and Running classes. The child classes of Workout inherit the unique id (for moving towards the pop-up on the map), date, distance, duration and coordinates.

The Running and Cycling classes calculate their own pace or speed (depending on which class). These classes are used to hold their specific data in an object, which then gets passed into the App class to render the object to the ui.
