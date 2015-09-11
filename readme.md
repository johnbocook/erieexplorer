
The ErieExplorer App 
===================

ErieExplorer showcases parks and activites surrounding  **Lake Erie Ohio**.
The project will allow featured locations and businesses to advertise and list events.

**Table of Contents**

* [Technology](#technology)
* [Installation](#installation)
* [Development](#development)

----------

Technology<a id="technology"></a>
-------------

> **Note:**
>  The development stack will be continuously changing as we perfect our workflow.

#### <i class="icon-shuffle"></i> [NodeJS](https://nodejs.org/)

Cross-platform runtime environment for developing server-side web applications in javascript.

#### <i class="icon-shuffle"></i> [AngularJS](https://angularjs.org/)

A structural framework for dynamic web apps. Uses HTML as the templateing language and extends the syntax to express the application's components clearly and succinctly. Angular also includes data binding and dependency injection.

* Angular Animate
* Angular UI Router

#### <i class="icon-desktop"></i> [Foundation](http://foundation.zurb.com/apps/)

A responsive front-end framework. Includes CSS3 [Flexbox](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Using_CSS_flexible_boxes) for application layouts and motion-ui.

#### <i class="icon-hammer"></i> [HammerJS](http://hammerjs.github.io/)

Library that can recognize gestures made by touch, mouse and pointerEvents. 

#### <i class="icon-exchange"></i> [Sass](http://sass-lang.com/)

Stylesheet language that extends CSS3, adding nested rules, variables, mixins, selector inheritance, and more.

#### <i class="icon-suitcase"></i> [Bower](http://bower.io/)

Package manager for Javascript libraries that allows you to define, version, and retrieve your dependencies

#### <i class="icon-food"></i> [GulpJS](http://gulpjs.com/)

Build system automating tasks: minification and copying of all JavaScript files, static images, capable of watching files to automatically rerun the task on changes.

#### <i class="icon-food"></i> [Other Plugins](#)

* **Gulp Uglify** - Minifies files with UglifyJS
* **Gulp Autoprefixer** - Auto add vendor prefixes to CSS 
* **Gulp Concat** - Concatenate CSS files, rebase urls and inlining @import
* **ngHtml2js** - Preprocessor converts HTML files to AngularJS templates
* **Gulp Sass** - Compile Sass to CSS
* **Rimraf** - Unix command rm -rf for Node
* **Yargs** - Command line options parsing
* **Front-Router** - Simplifies Angular Routes by defining route in view template.
* **Iconic Font** - Font based icon library
* **Tether** - Library makes absolutely positioned elements attach to another element.
* **Fast Click** - Removes 300ms delay between tap and click event.
* **Viewport Units Buggyfill** - Viewport hacks for Mobile Safari, IE3 and Stock Android

----------

Installation
-------------------

> **Note:**
> You will first need to have **Node**, **Git**, and **Ruby** on your machine.

```bash
// Clone repo to project directory
$ git clone https://github.com/johnbocook/ErieExplorer.git
```

```bash
// Change into directory
$ cd ErieExplorer
```

```bash
// Install bower and gulp
$ sudo npm install -g bower gulp
```

```bash
// Install Bundler
$ gem install bundler
```

```bash
// Install dependencies
$ sudo npm install 
$sudo bower install
```

```bash
// Run the app
$ npm start
```

This will compile the Sass and assemble the  application. **Now go to `http://localhost:8085` in your browser to see it in action.**  When you change any file in the `client` folder, the appropriate Gulp task will run and build new files.

----------

**Development**
-------------------
All development assets are located in the **/client** directory. When npm is started, all assets are pulled from that directory, parsed and placed into the **/build** directory. This is where the actual application is served from. 

<i class=" icon-attention"></i> **Do Not Modify /build** - Any code changes you make will be auto-processed by the watcher and and auto-loaded from **/client** to **/build**. Your browser will then auto-refresh.


**[<i class="icon-thumbs-up-alt"></i>](#) Pull Requests Encourged!**

**Todo:**
- [x] Build Frontend 
- [ ] Setup MongoDB database
- [ ] Build backend with Meteor

