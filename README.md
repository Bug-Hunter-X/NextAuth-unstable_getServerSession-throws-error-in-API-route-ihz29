# NextAuth unstable_getServerSession Error in API Route

This repository demonstrates a common error encountered when using `unstable_getServerSession` from the NextAuth.js library within an API route in Next.js.  The issue arises from incorrect usage or missing configurations leading to unhelpful error messages.

The `bug.js` file contains the problematic code, while `bugSolution.js` offers a corrected implementation.

## Steps to Reproduce

1. Clone this repository.
2. Install dependencies: `npm install`
3. Run the development server: `npm run dev`
4. Attempt to access the API route (e.g., `/api/protected`). You should see the error.
5. Refer to `bugSolution.js` for the corrected version.

## Problem and Solution

The core problem lies in how the `unstable_getServerSession` is handled, especially related to the context provided. The solution focuses on ensuring appropriate handling of `req` and `res` objects and proper configuration of NextAuth.