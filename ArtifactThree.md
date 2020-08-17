# Artifact Three - Databases 

The artifact selected for the databases category is an Android app for a fake local coffee shop. This app was created in an introduction to mobile development class at Southern New Hampshire University. I chose this artifact because I am interested in mobile app development, and it can demonstrate many of my skills regarding databases, along with providing opportunities to expand my knowledge. The app already implemented SQL databases, and I knew that I could add complexity to it. Another reason I chose this artifact is that I wanted to add the Firebase database API when initially developing this app, but I did not have the time in that class. The menu database and current order databases allowed me to demonstrate my abilities with SQL. The Firebase database allowed me to demonstrate my skills, writing and reading to a NoSQL database, APIs, and nested recycler views. 

### Showcased Skills

- Working with Firebase authentication and database APIs

- NoSQL database write and read

- Adding photos to SQL database

- Creating nested recycler views

### Demonstration of the database features of the app

<iframe width="420" height="315" src="https://www.youtube.com/embed/LYBB8XvHNtk" frameborder="0" allowfullscreen></iframe>

### Enhancements 

- Created a firebase database

- Implemented Google API

- Allowed the user to login using Facebook or Google and authenticated the user through Firebase

- Checked for user existence in the database, created a new user profile if it did not exist

- Added a continue as a guest option to bypass creating a profile and storing past orders

- Added the user's current order under the user's profile in Firebase when they place the order

- Retrieved the orders from the current user's profile and displayed them in a nested recycler view

- Updated SQLite menu database to include a photo of each item

### Reflection

When developing the database features, I learned how to store and retrieve photos from SQL and then display them in the user interface. The implementation of the Firebase database was the most challenging part for me because I did not have much experience with NoSQL databases before this. I learned how to create a Firebase real-time database linked to the app and read and write to it. Learning how to authenticate a user through Firebase Authentication was very allowed me to create a guest option and only allow specific people to access the Firebase database.

I struggled the most with understanding how to structure the database so that I could insert the order data and retrieve it to be displayed. After reading Firebase documentation, I decided to use the .push() function included in the Firebase API so that a new child was automatically created for each order, with them being ordered by when they were inserted. This allowed me to retrieve each order later. It was also challenging for me to figure out how to retrieve the lists of items, quantities, and subtotals from each order and displaying them in a nested recycler view. After retrieving and order from the database, it was added to the order model to extract the specific data from it. From there, I couldn’t get the lists of item names, quantities, and subtotals to display in the nested recycler view. I had to create lists in the activity displaying the parent recycler view to store the lists from the order model so that I could pass them to the nested recycler view.

[***Source Code for Android App***](https://clarissaworrell.github.io/ArtifactThree)

[Back](https://clarissaworrell.github.io/)
