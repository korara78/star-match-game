# star-match-game

## Overview

-A matching game. Select the number or sum of numbers to match the amount of stars displayed. There is a timer of 30 seconds. Guess all combinations before time expires.

-Based on Pluralsight course "React: Getting Started" By Samer Buna. This project gave me ongoing exposure to studying React useState and useEffect hooks. I was also able to gain exposure to the creation of developing a Custom Hook. 

This app is published at https://korara78.github.io/star-match-game/

## Logic

-The parent function component called StarMatch controls the state of gameID's as to refresh the state of the app upon each new game.

-A Custom Hook called useGameState contains the actual management of the app's state. It initalizes state and calls the setGameState functions to set the state. The Custom Hook useGameState takes timeLimit as an argument and returns the current state of stars, availableNums, CandidateNums, and secondsLeft. This Custom Hook also contains a useEffect Hook which handles the timer as well as a cleanup mechanism which resets the timer.   

-The function 'utils' contains the math science logic which allows the app to select a random amount of stars.

## Styling

-The body of the application is split into the 'left' side and 'right' side elements. The left side contains stars while the right contains number buttons. 

-@media Screen with max-width: 768px allows the application to be responsive for smart phones. The app maintains 100% width. The right side of the body will contain a background color of red to denote a smaller screen is being used as well as providing better contrast. T




