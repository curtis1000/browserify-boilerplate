# browserify-boilerplate

This is a simple demonstration of how you might setup a web project to use commonjs modules with browserify. 

###Setup###
  - ```npm install```
  - ```npm run watch```
  - Serve the ```/public``` directory
  
###Watch Script###
The [watch script](https://github.com/curtis1000/browserify-boilerplate/blob/master/package.json#L10) uses nodemon to monitor changes to *.js files in the /src directory, and calls the build script on changes.

###Build Script###
The [build script](https://github.com/curtis1000/browserify-boilerplate/blob/master/package.json#L9) runs browserify on the ```src/main.js``` entrypoint to our application, sending the output to ```public/build/app.min.js```. For minification, the browserify output gets piped through uglifyjs.
