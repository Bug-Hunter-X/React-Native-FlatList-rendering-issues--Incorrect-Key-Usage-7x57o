# React Native FlatList Key Error

This repository demonstrates a common error in React Native's FlatList component and its solution.  Using the index as a key in FlatList can cause incorrect rendering and unexpected behavior.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides the corrected implementation.

## Problem

Incorrectly using the index as a key in `FlatList`'s `renderItem` function can result in rendering inconsistencies, particularly when data updates occur. React Native may reuse the same index for different items, leading to incorrect data display or component updates.

## Solution

The correct approach is to use a unique identifier for each item in your data array as the key.  This ensures that React Native correctly identifies and manages each item in the list, even when the data changes.

## How to run

1. Clone the repository.
2. Run `npm install` or `yarn install`.
3. Run `npx react-native run-android` or `npx react-native run-ios`.