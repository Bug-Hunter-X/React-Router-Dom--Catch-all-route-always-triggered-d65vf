# React Router Dom Catch-all Route Issue

This repository demonstrates an uncommon issue with React Router Dom's catch-all route (`path="*"`). The catch-all route is unexpectedly triggered even when other routes should match.

## Problem
The provided code uses React Router Dom v6.  The catch-all route is always triggered, overriding any other route matches. This happens even when other routes are defined before the catch all route. 

## Solution
The solution involves carefully ordering and structuring routes within the React Router Routes component.  Avoid placing the catch-all route at the beginning, ensure the catch-all route is placed last and that all other routes that need to be matched are correctly defined.

## How to reproduce
Clone the repository and run `npm install`. Then run `npm start` to run the application.  Observe the catch-all route is always displayed.

## How to fix
Examine and review the solution in the `AppSolution.js` file for the corrected implementation.