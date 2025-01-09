# React Native FlatList Key Prop Issue

This repository demonstrates a common error in React Native's FlatList component: using incorrect or missing `key` props.  This can lead to unpredictable rendering behavior.

## The Problem

When the `key` prop is missing or improperly set, FlatList struggles to identify individual items during updates. This results in items not rendering correctly, extra items appearing, or items not updating properly.

## The Solution

Always provide a unique `key` prop for each item in the data array passed to FlatList.  This key should uniquely identify each item within the data set. It is often best to use the item's ID if available. The solution file shows the corrected implementation.

## How to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run `npx react-native run-android` or `npx react-native run-ios`.
4. Observe the buggy behavior in the initial rendering.
5. Observe the correct behavior after applying the solution from `bugSolution.js`.
