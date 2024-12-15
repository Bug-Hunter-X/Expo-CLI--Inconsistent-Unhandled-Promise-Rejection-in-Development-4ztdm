# Expo CLI: Inconsistent Unhandled Promise Rejection in Development

This repository demonstrates an uncommon bug encountered in Expo CLI development mode. The app crashes with an 'Unhandled promise rejection' error, lacking a clear stack trace for debugging. The issue's inconsistency makes reproduction challenging.

## Bug Description

The application, a simple Expo project, intermittently crashes during development. The error message in the console indicates an unhandled promise rejection, but doesn't offer specifics about the source or cause. This lack of detailed error information significantly hinders debugging efforts.

## Reproduction Steps

1. Clone the repository.
2. Navigate to the project directory.
3. Run `expo start`.
4. Observe the app's behavior.  The crash may occur at any time or may not reproduce at all.

## Potential Causes

While the exact root cause remains elusive, potential suspects include:

* **Asynchronous operations:**  Unhandled promises from background tasks or network requests.
* **Expo module interactions:** Conflicts or unexpected behavior within Expo modules.
* **Development environment issues:** Problems specific to the Expo development server or underlying system.

## Solution

The provided solution file, `bugSolution.js`, includes a possible fix that may resolve the issue (though this is dependent on the specific cause of the error).  Examine this file for details and adapt it as necessary for your circumstances.

## Note

The nature of this bug makes it highly context-dependent.  The exact cause and solution may vary based on your project's codebase and setup. This is merely one potential instance and solution.