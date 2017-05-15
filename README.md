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


Week 5 we added the the animationHandling class and the InventoryManagement class, which is an inner class for event handling.  Additionally, we added three buttons to the main GUI.  The first button displays the current inventory of the vending machine.  The second button demonstrates animations of the items in the vending machine falling into a basket, which will be implemented in the final dispenser GUI.  The third button is the start of the boss GUI.  It currently allows for the user to adjust item quantities but will later be expanded to allow for name, category, and price adjustments.
