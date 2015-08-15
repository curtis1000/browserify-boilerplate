# Browserify Boilerplate

This is a simple demonstration of how you might setup a web project to use commonjs modules with browserify. 

###Setup###
  - ```npm install```
  - ```npm run watch```
  - Serve the ```/public``` directory
  
###Watch Script###
The [watch script](https://github.com/curtis1000/browserify-boilerplate/blob/master/package.json#L9) uses watchify (which requires browserify in its dependencies) to monitor changes to ```src/main.js```, and runs browserify on changes.
