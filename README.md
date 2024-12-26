# Next.js 15 Runtime Error: Accessing Non-Existent Variable

This repository demonstrates a runtime error in a Next.js 15 application caused by accessing a non-existent variable within a component.  The error is not caught by Next.js's error boundaries, resulting in a full page crash. The solution shows how to handle this using error boundaries.

## Bug

The `pages/about.js` file attempts to access a variable (`nonExistentVariable`) that hasn't been declared or initialized. This throws a runtime error.  Next.js error boundaries do not catch this by default, resulting in a broken application.

## Solution

The solution utilizes Next.js's error boundaries to gracefully handle and display a user-friendly message instead of the full page crash.  The `pages/aboutSolution.js` file demonstrates the implementation.

## Steps to reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm run dev`.
4. Navigate to `/about`.

You will see the error.
Then switch to /aboutSolution to see the fixed solution.