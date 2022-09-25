# 2048_game
UCB CS61B proj0

The intent of this project is to give you a chance to get familiar with Java and the various tools used in the course like the IntelliJ IDE and JUnit for writing and running unit tests. Though you’ll find many files and lots of code in the proj0 folder, your task only resides in Model.java and is constrained to just four methods.

In this project, you’ll be building the core logic of this game. That is, we’ve already put together all the GUI code, handle key-presses, and a ton of other scaffolding. Your job will be to do the most important and interesting part.

Specifically, you will fill out 4 methods in the Model.java file which governs what happens after certain key-presses from the user.

The game itself is quite simple. It’s played on a 4*4 grid of squares, each of which can either be empty or contain a tile bearing an integer–a power of 2 greater than or equal to 2. Before the first move, the application adds a tile containing either 2 or 4 to a random square on the initially empty board. The choice of 2 or 4 is random, with a 75% chance of choosing 2 and a 25% chance of choosing 4.

The player then chooses a direction via their arrow keys to tilt the board: north, south, east, or west. All tiles slide in that direction until there is no empty space left in the direction of motion (there might not be any to start with). A tile can possibly merge with another tile which earns the player points.
![Game Example](/example-2048.gif)
