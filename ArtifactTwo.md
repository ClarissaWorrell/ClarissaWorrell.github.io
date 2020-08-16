# Artifact Two - Algorithms and Data Structures 

The artifact selected for the algorithms and data structures category is the same android app used in all of the artifacts. The app is for a fake local coffee shop business. It was initially created in a previous course at Southern New Hampshire University. I chose this artifact because mobile app development is something that I am passionate about and I knew it would allow me to demonstrate the skills I already had, along with providing many opportunities to learn new skills. The ordering system is the main feature that allowed me to showcase my abilities in algorithms and design. The process of displaying the data along with pass data from one class to another involved algorithms. This artifact is very intertwined with the databases artifact as many of the data structures were implemented to store data from the databases or insert data into them. 

### Showcased Skills

- Hashmap

- Lists

- Arrays

- Converting data types 

- Algorithms

### Demonstration of the algorithm and data structure features of the app

<iframe width="420" height="315" src="https://www.youtube.com/embed/lvSkIw2MLGM" frameborder="0" allowfullscreen></iframe>

### Enhancements 

- Redesigned the menu and current order displays

- Converted photos to byte array from bitmap to insert them into the SQL database, converted back to bitmap when retrived

- Added quanitiy options with constraints to the menu for each item using plus and minus buttons so that the user can't enter invaild input

- Checks for existance of an item in the current order database and then either adds a new item or updates the quantity of an existing item

- Stored the calculated subtotal of each item in a list

- Used a for loop to iterate through the list of subtotal and calculate the total price of the order

- Create a changing text view to display the total price of the order

- Updated the recycler view for the current order in realtime when an item is deleted

- Stored the data from the current order in lists and added those lists to a hashmap to be inserted in the Firebase database 

### Reflection

While making these enhancements I learned about how and when photos can be added to SQL databases and the data structures used to store them, how to set a changing text view in a recycler view item, how to update a recycler view in real-time, and how to use methods to pass lists from an adapter activity to an app activity rather than using serialization which slows down the app. I also learned many other smaller skills along the way such as which displays and constraints to use in android displays, how to always have a float display two decimal places, and many others. There are many skills that I learned while researching how to do things that I didn’t end up using but I now have the knowledge for later. 

The biggest challenge I faced was deciding how to store the photos for the menu items. After doing lots of research I determined that it was better to store the images in the database using blob rather than storing them on the device and putting the file path in the database because there are only a few images and the file sizes are small. According to SQLite it is faster and uses less storage to put the images in the SQLite database when using small image file sizes (2017). I converted the photos from bitmap into bytes to insert them into the database and then converted them back to bitmap when they are retrieved to be displayed. I only used one photo for all of the items because the source must be citied at the bottom of the screen and use multiple pictures would clutter the screen. The other aspect I struggled with was implementing the quantity option in each item of the recycler view. When I originally added this feature, the quantity was updating for all of the menu items, rather than just the item that the user was currently clicking which created problems when adding items to the order. I fixed this by retrieving the value of the current quantity text view each time the user increases or decreases the quantity and then updating the quantity text view of the current item.

Reference: SQLite. (2017, June 05). 35% Faster Than the Filesystem. Retrieved from https://www.sqlite.org/fasterthanfs.html

[***Source Code for Android App***](https://clarissaworrell.github.io/ArtifactThree)

[Back](https://clarissaworrell.github.io/)
