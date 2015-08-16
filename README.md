# Browserify Boilerplate

This is a simple demonstration of how you might setup a web project to use commonjs modules with browserify. 

###Setup###
  - ```npm install```
  - ```npm run watch```
  - Serve the ```/public``` directory
  
###How It Works###
The [watch script](https://github.com/curtis1000/browserify-boilerplate/blob/master/package.json#L9) uses watchify to monitor changes to the app's entrypoint ```src/main.js``` (or any modules referenced thereon). 

When a change is detected, watchify will run browserify which compiles source code to ```public/build/app.js```. 

Additionally, the exorcist module is utilized in the build step to generate a source map for chrome debugging.
