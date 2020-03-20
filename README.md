# BattleShip
 
This project aims to develop a Battleship game using Kotlin programming language.
BattleShip is a board game where to win you have to be the first to sink all 5 ships of your opponent's ships.

## Getting Started

If you've forked a copy of this Repo, don't forget to:
1. Set up your own Firebase project with a real google-services.json 
2. Enable Email/Password Sign in with Firebase Authentication 
3. Enable Firebase Realtime Database.

Use the following rules for the Database so only authenticated users can access/write data:
```json
{
  "rules": {
    ".read": "auth != null",
    ".write": "auth != null"
  }
}
```
### Features implemented in this project
- Manual Ship Placing
- Random Ship Placing
- Play Live
- Two-player
- Basic Graphics

### Designed the project using:
- Object Oriented approach, developing 'real world' entities such as Player, Board, Fleet of Ships, Score etc.
- Model-View-ViewModel design pattern to separate concerns between the View, the Data and the Logic.
- Data Structures: 
  .The Board is a two-dimensional array which elements can be accessed by their x and y coordinates.
  .The Group of Ships (the fleet) is a arrayList in the Board class.
  .etc.

### Screens in this project
- MainActivity to welcome the Player
- LoginActivity to login using Email/Password (using Firebase Auth and Firebase-UI)
- RoomsActivity to choose between creating a Room + waiting for the second player, or choosing a Room + joining a player
- SetupActivity to place the ships on the Board (Randomly or Manually)
- GameActivity to shoot on the opponent's board


  




