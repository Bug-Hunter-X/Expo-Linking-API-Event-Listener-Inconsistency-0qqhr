# Expo Linking API Event Listener Inconsistency

This repository demonstrates a bug in Expo's `Linking` API where the event listener for deep links (`Linking.addEventListener`) does not always trigger reliably.  This can lead to deep links being missed, causing unexpected behavior in your application.

## Bug Reproduction

The `linkingBug.js` file contains code that reproduces the issue. You'll need to set up an Expo project to run this code.  The code attempts to listen for a specific deep link and logs a message when it's received.  However, you'll find the listener doesn't consistently detect the link. 

## Solution

The `linkingBugSolution.js` file provides a potential solution that uses a combination of techniques to make the deep link handling more robust.  These techniques include using the `Linking.getInitialURL` and implementing timeout mechanisms to increase reliability.

## Contributing

Contributions are welcome! If you have a better solution or more details on the root cause of the problem, please open a pull request.