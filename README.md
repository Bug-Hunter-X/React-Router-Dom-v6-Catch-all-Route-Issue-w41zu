# React Router Dom v6 Catch-all Route Issue

This repository demonstrates a common issue encountered when using the catch-all route (`/*`) in React Router v6. The problem is that the catch-all route is always triggered, regardless of whether a valid route exists.

## Bug Description

The `/*` route in `App.js` is intended to handle 404 errors. However, it always matches, even when navigating to other routes like `/` or `/about`.

## Solution

The solution involves placing the catch-all route at the end of the `Routes` component. This ensures that other routes are checked first before the catch-all route is considered.

## Setup

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
