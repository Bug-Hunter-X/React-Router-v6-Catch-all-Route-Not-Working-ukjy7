# React Router v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`path="*"`) in React Router v6.  The catch-all route is intended to handle any route that doesn't match other defined routes, but in certain scenarios, it may fail to work as expected.

The `App.js` file contains the problematic code. The `AppSolution.js` provides a fix.

## Problem

The catch-all route does not handle routes that don't match other defined routes. For example, navigating to `/invalid-route` does not display the 404 page.

## Solution

The solution involves ensuring the catch-all route is the last route defined within the `Routes` component. The correct order of routes within `Routes` is crucial for its functionality.