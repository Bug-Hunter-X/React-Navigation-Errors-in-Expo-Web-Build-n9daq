# React Navigation and Expo Web Compatibility Issue

This repository demonstrates a common error encountered when using React Navigation within Expo's web platform.  React Navigation relies on native modules for certain functionalities that are unavailable in a web browser environment. This leads to runtime errors during the web build process.

## Problem Description

The issue arises when components within a React Navigation structure attempt to access or utilize native-only modules.  This often results in `TypeError` exceptions or similar errors indicating that an expected method or property is undefined.

## Solution

The solution involves careful consideration of which components and navigation features are used.  Any component relying on native modules should be excluded from the web build process, either by conditional rendering or by utilizing web-compatible alternatives.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` or `yarn install`.
3. Attempt to start the Expo web build (`expo start --web`).
4. Observe the error in the browser's developer console.

## Fixing the issue
Refer to the solution content to implement fixes.  This generally involves conditionally rendering components or employing web-specific navigation libraries.