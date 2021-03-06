# CST-135-Vending_Machine_Application
Class Project

Authors: Michel Weaver, Nicholas Robertson, Charles Witten, Rose Marie Lizama

Background: This project is a class project for CST-135. We are tasked with creating a vending machine application and have currently created the Dispenser Class which houses most of the functionality of the actual vending machine. We have created accompanying Product Class, Snack and Drink subclasses, and then populated the Dispenser with Product objects to be displayed.


Week 3 we have added the comparable interface to both the Snack and Drink classes so that these objects can be sorted with regards to one another. 

Currently the project is still under construction.

Approach: We are creating simple classes with data fields that are used in the overarching project. We have hardcoded a set number of objects into the Dispenser to begin with.

Use: Currently the user needs access to Eclipse, or a JDK that can run the .java files. Vending_Machine_Application.7z contains the project files. Within the project, Main.java contains the main method for execution. Once the main method is called the user will then receive a list of all stocked products. This will change as the project calls for it.

The main method now also calls the compareTo method of the snack class and displays that it works in regards to two separate chip objects.


Week 4 we created a graphical user interface for the dispenser class and created a TransactionProcessing class.  The GUI displays the four categories of food items along with a button for each.  Upon clicking the button, the items for the category are displayed along with their price and quantity.  The user can then purchase items, and after clicking the Done button, the purchased items are displayed along with the total cost of the transaction.

The new TransactionProcessing class takes in a Product object for each transaction and stores it in an ArrayList.  The total amount of money used in the transaction is stored, as well as the money remaining to purchase more items.


Week 5 we added the the animationHandling class and the InventoryManagement class, which is an inner class for event handling.  Additionally, we added three buttons to the main GUI.  The first button displays the current inventory of the vending machine.  The second button demonstrates animations of the items in the vending machine falling into a basket, which will be implemented in the final dispenser GUI.  The third button is the start of the boss mode GUI.  It currently allows for the user to adjust item quantities but will later be expanded to allow for name, category, and price adjustments.


Week 6 we added the following classes: GlobalInventoryManagement, Restock, and ErrorMessage.

The GlobalInventoryMangement class handles the processing of .csv files, spreadsheets which contain all the information for a new vending machine.  The class reads the file, processes each cell in the spreadsheet, and adds a Dispenser object to an ArrayList containing all the dispensers.  The class also has the ability to sort items within the dispenser by name and quantity, as well as recursively search for items by name.

The Restock class determines whether a dispenser needs to restock any of its items, returning an ArrayList of Products which are below the threshold of three or fewer items.

The ErrorMessage class is used to display an error dialog box whenever errors occur, such as invalid inputs by the user or an incorrectly formatted .csv file.  It contains one method called display(), taking in a message String and a title String.

The Main.java file contains two methods demonstrating the new functionality in this week's milestone.  The inventoryTest() method demonstrates the GlobalInventoryManagement class, testing the sort feature and recursive search and then outputting the results to the console.  The displayGUI() method shows the user interface as it currently stands, containing the new Dispenser Manager, which allows the user to import .csv files to create new dispensers, display a list of items needed to be restocked, and manage products in a dispenser.  The user can modify an item's name, quantity, and price.


Week 7 was the final week in developing our application.  We added an Adjust Money feature in which the customer can add or subtract money with which to purchase items from the dispenser.  We also added a Customer Animation feature, which reads from a .CSV file, creating a queue of customers and an item to be purchased.  If the item is not available, the customer chooses a new item at random.  If that item is not available, this process continues until five failed attempts.  This queue of customers is displayed visually, with each customer going up to the machine one at a time, with their purchasing requests displayed in a window to the right.

To run the application, download and export the "Virtual Vending Machine.7z" file.  After exporting, find and execute the runnable Java applet called "Virtual Vending Machine.jar".


Individual contributions:

Nicholas Robertson:  Most of my work was in designing the GUI, implementing the existing classes and making changes to the classes as necessary.  I created the following graphical interfaces: Selection by Category, Display all Inventory, Adjust Money, and Dispenser Manager.  I also created the ErrorMessage class and used it to validate data entry, such as the importing of .CSV files as new dispensers and inputting numerical values into text boxes.  I also expanded the GlobalInventoryManagement class to process an ArrayList of Dispenser objects, allowing for the management of multiple vending machines.

Michael Weaver: I worked in tangent with Nicholas to create various parts of the project, picking up what slack I could when I could. I created AnimationHandling (aside from the resetAnimationTest, which Charles did), the Product and subclasses were all designed by me and had their finishing details added by the others, ProcessCustomerQueue and CustomerVending are both mine with help from Nicholas to finish them off, chunks of the DispenserGUI class were designed by me (including the vendTest), as well as the images of the project.
