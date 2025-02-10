# Undeclared Variable Bug in Next.js 13

This repository demonstrates a common error encountered when upgrading to Next.js 13 due to the introduction of strict mode.  Strict mode in JavaScript helps catch common coding mistakes.  If you're upgrading from a previous version of Next.js and have undeclared variables, your application will throw an error.

## Problem

The `about.js` file contains an undeclared variable `a`, which will cause a runtime error in strict mode.  This is because strict mode prevents the use of implicitly declared variables (those not explicitly declared using `var`, `let`, or `const`).

## Solution

The solution involves ensuring all variables are explicitly declared before use. The updated `about.js` demonstrates this fix.

## Reproduction

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm run dev` to start the development server.
4. Navigate to `/about` – you'll observe the error being thrown unless you've made the changes.
