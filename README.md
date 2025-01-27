# Firebase Offline Persistence Issue

This repository demonstrates a bug encountered with Firebase's offline persistence.  Data is inconsistently saved across sessions, even with offline persistence enabled. The problem is intermittent and doesn't produce obvious error messages in the console.

## Bug Description

The application uses Firebase Realtime Database. While offline persistence is enabled, data is not always persisted across sessions.  This leads to data loss in seemingly random instances.

## Solution

The solution explores potential causes like improper initialization or race conditions in data handling, providing an improved method to ensure data is reliably written to the database. The fix involves carefully managing the database operations and potentially incorporating error handling to catch subtle issues.

## Setup

1. Clone the repository.
2. Install dependencies: `npm install`
3. Configure your Firebase project.
4. Run the application: `npm start`

## Files

- `bug.js`: Demonstrates the original, flawed code.
- `bugSolution.js`: Shows the improved, corrected code.