# Set_Card_Game

Multithreaded version of the well-known game "Set". This is an assignment part of the SPL course in my Bachelor's degree. I have implemented the "Dealer", "Table", and "Player" classes, along with game logic.

# About

Game Flow : The game contains a deck of 81 cards. Each card contains a drawing with four features (color,number, shape, shading). The game starts with 12 drawn cards from the deck that are placed on a 3x4 grid on the table. The goal of each player is to find a combination of three cards from the cards on the table that are said to make up a “legal set”. The game ends when there is no legal sets in the deck.

Supply the main thread that runs the table logics, the main thread that runs the "Dealer" that manages the game flow, and a single thread for each player.

# Installing and Running the Game

1. Make sure Java is installed (1.8 or later).
2. Download all of the files.
3. Navigate to "set-game-main\target\classes\config.properties". You can change the game settings as you wish:
  - HumanPlayers - Amount of human players.
  - ComputerPlayers - Amount of computer players.
  - Hints - True/False - show legal sets currently visible on the table.
  - PlayerNames - players names, separated by `", "` - example is given.
    
    Note: Modify config.properties, not config_Original.properties.
4. Navigate to "set-game-main\src\main\java\bguspl\set\Main.java" and run the project.

# How To Play
1. At the bottom of the config.properties file, we define the 12 buttons for 2 human players. 
Each key represents a slot. Each player controls 12 unique keys on the keyboard as follows.   
2. When you press 3 different buttons, if the 3 form a set, you receive a point. Otherwise, you incur a penalty for a few seconds (as defined in the settings).
3. If you press incorrectly, first press again the slots you pressed and wish to unpress.
4. The winner is the player with the most points when no more sets are available in the deque.

# Main features 
1.	Use locks and atomic variables to manage the threads. 
2.	Employ synchronization concepts for a "Fair" game.
3.	Fully support human players and computer players.

# Screen Shots
| | |
|:-------------------------:|:-------------------------:|
|<img style="max-width:200px; width:100%"  src="https://github.com/GalEden99/SPL_assignment2-Set_Card_Game/blob/master/images/initial%20table.png" alt="initialTable" >|<img style="max-width:200px; width:100%"  src="https://github.com/GalEden99/SPL_assignment2-Set_Card_Game/blob/master/images/table%20with%20tokens.png" alt="tableWithTokens" >

