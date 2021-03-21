Student name: Ali Abbas Naqvi
Student number: 200788667

Now complete the statements below for each level you wish to be marked. Replace all text in square brackets.

LEVEL ONE

My code demonstrates inheritance in the following way...

I have a superclass called Character

This superclass is extended into at two subclasses called Player, NonPlayer, Target, Staff, Bodyguard.
For each of the named subclasses complete the following...

Subclass 1.

Subclass Player extends the superclass by adding at least one property and its getters and setters. The name(s) of the added properties are health, visibility, and inventory.

These new properties are used by the subclass in the following way: 
Health was added as a life system for the player so when they fail in an action, they are punished through losing health. If they lose all their health, the game is over.
This can be seen in lines 117, 128, 146, and 157 in which health is deducted for failing to escape or failing to subdue someone. 
Visibility was added as a stat to increase/decrease the probability of a player escaping a room.
This can be seen in line 110 in which visibility is factored into the player's escape chance.
Inventory was added as a place to store items picked up by the player so it can be accessed to add on the appropriate stats.
This can be seen in lines 36-48, 56-70, 78-88, and 94-106 in which inventory is used in a for loop to access the contents to add the stats onto the player.

Subclass Player extends the superclass by overriding the following methods (there must be at least one): escape() at 108-133, modifyDefenseLevel() at 78-92, and modifyAttackLevel() at 94-106.

These overridden methods are used in the working code in the following places: File: Game, Lines: 172, 423-432, and 394-403.

Subclass 2.

Subclass NonPlayer extends the superclass by adding at least one property and its getters and setters. The name(s) of the added properties are conscious, alive, escaped.

These/this new properties/property are used by the subclass in the following way: 
These three properties were added to serve as possible states for non player characters to be in during the course of the game.

Subclass NonPlayer extends the superclass by overriding the following methods (there must be at least one): N/A
These overridden methods are used in the working code in the following places: N/A

Subclass 3.

Subclass Target extends the superclass by adding at least one property and its getters and setters. The name(s) of the added properties are distanceFromWeapon.

These/this new properties/property are used by the subclass in the following way: 
The target in the game is depicted as walking back and forth thus the property distanceFromWeapon simulates his distance from potential weapons in his room that he has access to as he is walking around. It used in line 22 to check if the target is able to reach a weapon, if he can reach a weapon he is given an advantage in the attack() method which serves as a 'boss' mechanic.

Subclass Target extends the superclass by overriding the following methods (there must be at least one): attack() at line 32-57, printDescription() at line 59-82

These overridden methods are used in the working code in the following places: File: Game, Lines: 69, 53

Subclass 4.

Subclass Staff extends the superclass by adding at least one property and its getters and setters. The name(s) of the added properties are braveness

These/this new properties/property are used by the subclass in the following way: This property was added to simulate the braveness of a staff member who would try to escape rather than fight when given the chance.

Subclass Staff extends the superclass by overriding the following methods (there must be at least one): escape() at 33-41, printDescription() at 43-68

These overridden methods are used in the working code in the following places: File: Game, Lines: 210-222, 245-247 || File: Room, Lines: 51

Subclass 5.

Subclass Bodyguard extends the superclass by adding at least one property and its getters and setters. The name(s) of the added properties are distracted

These/this new properties/property are used by the subclass in the following way: Bodyguards serve as a tougher opponent for the player than staff but can be made vulnerable if they are distracted. This can either happen randomly as a room is generated with a distracted bodyguard or through a player tossing a coin. A distracted bodyguard is easier to subdue and easier to escape a room from.

Subclass Bodyguard extends the superclass by overriding the following methods (there must be at least one): stopEscape() at 20-37

These overridden methods are used in the working code in the following places: File: Game, Line 168


LEVEL TWO

Polymorphism consists of the use of the Substitution principle and Late Dynamic binding.

In my code, polymorphism is implemented in at least two places…

Example 1.

The substitution principle can be seen in use in Game on lines 490-506. The name of the superclass used in this example is Item and the subclasses used are Coin, Food, and Clothes.

Late dynamic binding can be seen in Game on line 390 & 419.

This is polymorphism as firstly the substitution method is seen used on lines 488-504 to create objects of the type superclass Item but of subtype of the subclassess Coin, Food and Clothes. Late dynamic binding can be seen with this objects on line 390 & 419 as the superclass method stats() is used and is overriden by the subtype's stats() method from the subclasses Food and Clothes.

Example 2.

The substitution principle can be seen in use in Game on line 488-504. The name of the superclass used in this example is Item and the subclasses used are Food, Clothes, and Coin.

Late dynamic binding can be seen in Room on lines 63.

This is polymorphism as firstly the substitution method is seen used on lines 488-504 to create objects of the type superclass Item but of subtype of the subclassess Coin, Food and Clothes. The late dynamic binding occurs as the superclass' printDescription is overriden by the subtype's printDescription method from all 3 subclasses.