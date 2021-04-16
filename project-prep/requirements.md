# Project Prep 4 - Software Requirements

## Vision

- **What is the vision of this product?** A React Native mobile game that allows a user to play a game of sinky ship against a computer opponent. The game will be interactive through a mobile device  and work with randomly generated sinky ships.
- **What pain point does this project solve?** Allows for a novel way to enjoy your free time.
- **Why should we care about your product?** Takes a classic game and makes it more enjoyable and dynamic.

## Scope In/Out

### In

- Use React Native to create a visally appealing mobile application of Sink Ship.
- Utilize socket.io to help facilitate multiple simultaneous gameplay connections.
- Give computer ability to make randomized choices and also ability to aim for ships once they have been hit once.
- Allow for progressively more diffcult AI opponent.
- Create an algorithm for computer selection of targets on the board.
- Utilize the power of graphs for better gameplay.
- Authentication

### Out

- Machine Learning
- VR
- AWS
- IOS

## Minimum Viable Product (MVP)

- Installable mobile application with React Native, that is utilizing socket.io to facilitate server connection. Randomly generated battlefield with sinky ships. Improve gameplay with graphs to make it more dynamic. Create tests to prove functionality of game. Application is deployed live. A coherent visual design with cohesive color scheme.

- Stretch goals: database for high scores, premium content (extra ships), expandable battlefield/playfield, extra game mechanics (mines, torpedos), Home screen with Splash Image with basic instructions. Game over with a swashbuckling pirate mocking you if you lose or win.

## Functional Requirements

- As a user I would like to be able to interact with the game and have it be visually appealing because I would find it more engaging
- As a user I want the application to be able to notify the server of my movements and send me the output after my opponent has moved and vice versa so that I can play the game
- As a player I want the computer to be able to prove a worthy adversary because that will be more fun
- As a user I want to be able to download the application as an mobile application because it will be more engaging
- As a user I would like to play against a computer opponent that is better than just choosing random selections and is harder to play against because it uses an algorithm for selecting targets

### Data Flow

![image](/assets/sinkyShipDomV2.png)

## Non-Functional Requirements

- Security: open source
- Usability: React Native app for install, use on a mobile device, minimal setup, documentation
- Testability:
  - Utilize jest to test ability for user input and also console log spy to test console output
  - Use jest to test emitting and publishing of messages with socket.io
  - Create jest test to be able to make sure the computer can aim for a space next to a ship once it has been detected
  - Make sure a user is able to successfully download and use the application on their mobile device
  - Computer using algorithm should be more effective at game than when using random selection