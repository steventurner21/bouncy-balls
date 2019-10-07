# Bouncy Balls [![Build Status](https://travis-ci.org/steventurner21/bouncy-balls.svg?branch=master)](https://travis-ci.org/steventurner21/bouncy-balls)

Bouncy Balls is a web application that creates a ball where you click with a random velocity, available [here](http://bouncy-balls.surge.sh/). It's written in ES6, transpiled by babel, and packaged by webpack.

## Building

Builds are generated by Travis CI and uploaded to surge.sh on push to master

To build the project locally using webpack, simply run `npm run build`. The generated files are stored in the dist directory.

## Testing 

Testing the project can be done by simply running `npm test`. The tests are written using jest and are named {component}.test.js

## Developing

### Project Structure

The project is structured as follows:

```
.
+-- dist (contains built files)
|   +-- index.html (index page file that loads the built javascript)
+-- node_modules (not committed, generated by npm install)
+-- src (contains all js source files)
|   +-- Component Folders (named with upper camel case, contains individual ES6 classes along with their associated tests)
|   |   +-- Component.js (the main code for that component)
|   |   +-- Component.test.js (the test file for that component)
|   |   +-- index.js (simply imports the module and exports it to make importing the component in other components easier)
|   +-- index.js (the main entrypoint for the javascript code)
+-- .babelrc, package.json etc (project level config files)
```
