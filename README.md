# React useEffect Hook Bug

This repository demonstrates a common error in using React's `useEffect` hook:  incorrectly specifying the dependency array, leading to unexpected behavior.

## Bug

The `bug.js` file contains a component that uses `useEffect` to log the current count. However, the dependency array is empty (`[]`), causing the effect to run only once, even though the count changes.  This leads to the count not being logged accurately after each click.

## Solution

The `bugSolution.js` file corrects this by including `count` in the dependency array. Now, the effect will run whenever `count` changes, providing accurate logging.

## How to reproduce

1. Clone this repository.
2. Navigate to the project folder.
3. Run `npm install` (or `yarn install`).
4. Run `npm start` (or `yarn start`).
5. Observe the console logs and the button behavior.