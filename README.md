# star-match-game

## Overview

-A matching game. Select the number or sum of numbers to match the amount of stars displayed. There is a timer of 30 seconds. Guess all combinations before time expires.

-Based on Pluralsight course "React: Getting Started" By Samer Buna. This project gave me ongoing exposure to studying React useState and useEffect hooks. I was also able to gain exposure to the creation of developing a Custom Hook. 

This app is published at https://korara78.github.io/star-match-game/

If github-pages is down check app on code pen https://codepen.io/kevin-orara/full/qBjaWqp

## Logic

-The parent function component called StarMatch controls the state of gameID's as to refresh the state of the app upon each new game.

-A Custom Hook called useGameState contains the actual management of the app's state. It initalizes state and calls the setGameState functions to set the state. The Custom Hook useGameState takes timeLimit as an argument and returns the current state of stars, availableNums, CandidateNums, and secondsLeft. This Custom Hook also contains a useEffect Hook which handles the timer as well as a cleanup mechanism which resets the timer.   

-The function 'utils' contains the math science logic which allows the app to select a random amount of stars.

## Styling

-The body of the application is split into the 'left' side and 'right' side elements. The left side contains stars while the right contains number buttons. 

-@media Screen with max-width: 768px allows the application to be responsive for smart phones. The app maintains 100% width. The right side of the body will contain a background color of red to denote a smaller screen is being used as well as providing better contrast. 


# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

### Code Splitting

This section has moved here: [https://facebook.github.io/create-react-app/docs/code-splitting](https://facebook.github.io/create-react-app/docs/code-splitting)

### Analyzing the Bundle Size

This section has moved here: [https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size](https://facebook.github.io/create-react-app/docs/analyzing-the-bundle-size)

### Making a Progressive Web App

This section has moved here: [https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app](https://facebook.github.io/create-react-app/docs/making-a-progressive-web-app)

### Advanced Configuration

This section has moved here: [https://facebook.github.io/create-react-app/docs/advanced-configuration](https://facebook.github.io/create-react-app/docs/advanced-configuration)

### Deployment

This section has moved here: [https://facebook.github.io/create-react-app/docs/deployment](https://facebook.github.io/create-react-app/docs/deployment)

### `yarn build` fails to minify

This section has moved here: [https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify](https://facebook.github.io/create-react-app/docs/troubleshooting#npm-run-build-fails-to-minify)
