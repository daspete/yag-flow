YAG Flow (yet another gulp workflow)
===============================
This is a quick gulp workflow for ES6 Javascript developers.


----------


Installation
------------

clone this project and then start

    npm install



----------


Babelify presets
----------------

 - ES2015
 - React


----------


Tasks
-----

***sass***

reads the file `styles.scss` from the `/src/sass/` folder and compiles it to `/public/css/styles.css`

***js***
	 
reads the file `app.js` or `app.jsx` (depending on the arguments passed to gulp) from the `/src/js/` folder and compiles it to `/public/js/app.js`

***images***

reads `JPG, PNG and GIF` files from the `/src/assets/images/` folder, optimizes them and pastes them into `/public/assets/images/`

***watch***

watches every change in the `/src/` folder and starts the right tasks, if there is a change


----------


Default task
------------

if you run

    gulp

everything is compiled and then watched, **browsersync** is also started at the **port 8089** and after every change, the browser will be refreshed.

if you run 

    gulp --react

the system needs a `app.jsx` file in the `/src/js/` folder.