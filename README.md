# TreasureHuntgame
Step 1.Create the Location class
Create a new Java class named Location and provide it with two private fields: name and description.
Create a constructor for the Location class that initializes these fields.
Create getter methods for the name and description fields.

Step 2: Create the Treasure class
Create a new Java class named Treasure with three private fields: name, description, and value.
Implement a constructor for the Treasure class that initializes these fields.
Create getter methods for the name, description, and value fields.

Step 3: Create the TreasureHuntGame class
Create a new Java class named TreasureHuntGame.
Define the main method:

Step 4: Declare and initialize data structures
Inside the main method, declare and initialize the different data structures(Map,list,set)
- create map locations with <String, Location> as kep value pair 

- create list treasures which containes list of treasure

- create set inventory which contains list of treasure

setp 5: Populate locations and treasures
Populate the locations map and the treasures list with a few initial locations and treasures of your choice.(eg locations.put("Beach", new Location("Beach", "You are on a beautiful beach with golden sands.")) treasures.add(new Treasure("Gold Coin", "A shiny gold coin", 10)))

Step 6: Implement the game loop
create string variable which stores the current location eg String currentLocation = "Beach";
Create a while (true) loop to keep the game running until the player decides to quit.

Step 7: Display the current location
Inside the game loop, retrieve the Location object for the current location.
Print the location's description.

Step 8: Prompt the player for actions(use scanner to take users input)
Display a menu for the player to choose from:
"Do you want to (1) Pick up a treasure, (2) Move to the next location, or (3) Quit? "

Step 9: Implement player choices
For choice 1, implement the logic for picking up a treasure.(showTreasures)
For choice 2, implement the logic for moving to the next location (You can prompt the player to enter the name of the location).
If a valid location is found, it sets currentLocation to the new location's name and informs the player that they have moved.
For choice 3, display the player's inventory, calculate the total value of the treasures, and end the game.(calculateTotalValue)

Step 10: Implement the showTreasures, showInventory, and calculateTotalValue methods 
- showTreasures: The method takes a parameter of type List<Treasure> treasures, which represents a list of available treasures in the game.use for loop tp traverse through each treasure . For each treasure, retrieve its name, description. this method makes it easier for the player to decide which treasure they want to pick up by selecting the corresponding number associated with each treasure.
- showInventory: is responsible for displaying the contents of the player's inventory. The method takes a parameter of type Set<Treasure> inventory. It starts by printing a header message: "Your Inventory:" to inform the player that the following list will display the contents of their inventory.It prints the details of each item in the player's inventory bt traversing through each inventory.
- calculateTotalValue : The calculateTotalValue method in the provided code is responsible for calculating and returning the total value of all the treasures in the player's inventory. 
