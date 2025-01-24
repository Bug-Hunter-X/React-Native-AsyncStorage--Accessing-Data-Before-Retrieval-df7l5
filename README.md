# React Native AsyncStorage Bug: Data Access Before Retrieval

This repository demonstrates a common bug in React Native applications when using AsyncStorage to store and retrieve data. The bug arises from attempting to access data before the asynchronous retrieval operation completes, leading to undefined values.

## Bug Description

The `AsyncStorageBug.js` file showcases the issue: data is accessed immediately after the `getItem` call, without waiting for the promise to resolve. This results in `undefined` being used, potentially causing errors or unexpected behavior.

## Solution

The `AsyncStorageBugSolution.js` file demonstrates the correct approach using `async/await`.  This ensures that the data is fully retrieved before being used, preventing the undefined value problem.

## How to reproduce the bug
1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Run the app with either the original buggy file (`AsyncStorageBug.js`) or the corrected file (`AsyncStorageBugSolution.js`).
4. Observe the differences in console logs and app behavior.
