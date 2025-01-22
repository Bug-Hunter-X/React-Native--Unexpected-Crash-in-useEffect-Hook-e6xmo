# React Native useEffect Hook Error

This repository demonstrates a common error encountered when using the `useEffect` hook in React Native functional components.  The error arises from attempting to access `this.state` within the `useEffect` callback, which is invalid in functional components.

## Bug Description

The provided code snippet uses `this.setState` within a `useEffect` hook inside a functional component. This is incorrect, as functional components do not have a `this` context or `state` property in the same way class components do.  This leads to a runtime error and the application crashes.

## Solution

The solution involves using the `useState` hook appropriately to manage component state within the functional component.