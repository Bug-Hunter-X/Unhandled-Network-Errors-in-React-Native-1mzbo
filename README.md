# Unhandled Network Errors in React Native

This repository demonstrates a common error in React Native applications: unhandled network errors.  Improper error handling when fetching data can lead to a poor user experience.

## The Problem

The `bug.js` file contains a component that fetches data from a remote API.  However, it doesn't handle network errors gracefully. If the API request fails, the application might crash or display a blank screen.

## The Solution

The `bugSolution.js` file provides a corrected version of the component. It uses a `try...catch` block to handle potential errors during the fetch operation. A `finally` block ensures the `loading` state is updated, regardless of success or failure.  This provides the user with feedback while improving app reliability.

## How to Run

1. Clone the repository.
2. Navigate to the directory in your terminal.
3. Run `npm install` to install dependencies.
4. Run `npx react-native run-android` (or `npx react-native run-ios`) to start the app on your device or simulator.