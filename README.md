# Emotion Semantic UI

CSS in JS implementation of Semantic UI using EmotionJS

## Development

This project primarily uses StorybookJS for development.

### Quick Start

1. `git clone` this project
1. `npm install`
1. `npm run storybook` or `npm run dev`

### Creating components

Make a new folder in the components folder, make sure the folder name is unspaced and Pascal Case (ExampleComponentName). Create a JS file with the same folder name (or appropriate variation).

Requirements

* Documented PropTypes and default props.
* Storybook examples in a `stories` subfolder.

### Project Structure

The goal is to keep the package as lightweight and minimal as possible, so there's not much to it. If you look at the `package.json`, you'll see a few dev dependencies like Babel, React, and Storybook. 

In terms of actual dependencies, we only have EmotionJS, since it's used in the actual components. React and react-dom are peer-deps (since the project's using this will be react-based).

#### Folder Structure

* /components/
* /components/ComponentName/
* /components/ComponentName/ComponentName.js
* /components/ComponentName/index.js - contains exports of all components in folder
* .babelrc - env and react Babel presets.