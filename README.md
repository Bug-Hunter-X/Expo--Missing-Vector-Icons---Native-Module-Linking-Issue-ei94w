# Expo Vector Icons Linking Issue

This repository demonstrates a common but often hard-to-diagnose problem in Expo projects when using `@expo/vector-icons`. The issue stems from a failure to properly link native modules, leading to missing icons or build errors. The error messages may not directly indicate the problem.

## Bug Description

When using `@expo/vector-icons` in an Expo project, icons might not render correctly, or the build process may fail.  The issue may not give a clear error message related to native module linking.

## Solution

The solution involves carefully verifying that the native modules for your chosen icon sets are correctly linked within both the iOS and Android parts of your Expo project. This typically requires the use of `expo prebuild` and possibly manual adjustments if `expo prebuild` doesn't fix the issue.

## Reproduction Steps

1. Clone this repository.
2. Run `npm install` or `yarn install` to install dependencies.
3. Attempt to run the app. The icons in `BugVectorIcons.js` will likely not render. 
4. See `SolutionVectorIcons.js` to solve the issue.