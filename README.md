# React useEffect Cleanup Function Not Running

This repository demonstrates a common issue with the React `useEffect` hook: the cleanup function not always running as expected.

## Bug Description
The provided `MyComponent` uses `useEffect` to log the current count and includes a cleanup function.  The issue arises when the component is unmounted or the effect is replaced. The cleanup function, which should log a message, doesn't always execute.

## How to Reproduce
1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs. The cleanup function message might not always appear when expected.

## Solution
The solution involves carefully examining the dependencies array in the `useEffect` hook.