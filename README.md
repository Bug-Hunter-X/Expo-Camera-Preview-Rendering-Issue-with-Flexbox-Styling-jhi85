# Expo Camera Preview Rendering Issue with Flexbox Styling

This repository demonstrates a bug in the Expo `Camera` component where applying `flex: 1` styling to the preview results in rendering issues. The camera preview may appear blank or distorted.  The issue seems linked to the interaction between the camera preview and the flexbox layout engine.

## Bug Description

When custom styling is applied to the Expo Camera component, specifically including `flex: 1` in the style object, the camera preview fails to render correctly. This leads to an empty screen or a distorted camera feed.

## How to Reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install`.
4. Run `expo start`.
5. Observe the blank or distorted camera preview.

## Solution

A workaround is provided in `bugSolution.js` that uses alternative styling techniques avoiding `flex: 1` to resolve the rendering issues.  This showcases a method to achieve a full-screen camera while avoiding the conflict.  A more robust solution would require a deeper investigation of the Expo Camera component's interaction with flexbox.