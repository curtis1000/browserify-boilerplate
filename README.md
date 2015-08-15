# Browserify Boilerplate

This is a simple demonstration of how you might setup a web project to use commonjs modules with browserify. 

###Setup###
  - ```npm install```
  - ```npm run watch```
  - Serve the ```/public``` directory
  
###How It Works###
The [watch script](https://github.com/curtis1000/browserify-boilerplate/blob/master/package.json#L9) uses watchify to monitor changes to the app's entrypoint ```src/main.js``` (or any modules referenced thereon). 

When a change is detected, watchify will run browserify which compiles source code to ```public/build/app.min.js```. There is an additional step through ```uglifyjs``` to add minification as well.
