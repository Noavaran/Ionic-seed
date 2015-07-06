# Ionic-seed — the seed for Ionic apps

This project is an application skeleton for a typical [Ionic](http://http://ionicframework.com/) hybrid mobile app.
You can use it to quickly bootstrap your Ionic hybrid app projects and dev environment for these projects.

The seed contains a sample ionic application and is preconfigured to install the Ionic
framework, Ionic Material and a bunch of development and testing tools for instant hybrid mobile app development gratification.

The seed app doesn't do much, just shows how to wire few controllers and views together. defaults icon and splash screen and also configuration xml file for both and ios.


## Getting Started

To get you started you can simply clone the ionic-seed repository and install the dependencies:

### Prerequisites

You need git to clone the ionic-seed repository. You can get git from
[http://git-scm.com/](http://git-scm.com/).

We also use a number of node.js tools to initialize and test ionic-seed. You must have node.js and its package manager (npm) installed.  You can get them from [http://nodejs.org/](http://nodejs.org/).

### Clone ionic-seed

Clone the ionic-seed repository using [git][git]:

```
git clone https://github.com/ali-pourzahmatkesh/Ionic-seed.git
cd ionic-seed
```

If you just want to start a new project without the ionic-seed commit history then you can do:

```bash
git clone --depth=1 https://github.com/ali-pourzahmatkesh/Ionic-seed.git <your-project-name>
```

The `depth=1` tells git to only pull down one commit worth of historical data.

### Install Dependencies

We have two kinds of dependencies in this project: tools and ionic framework code. The tools help us manage and test the application.

* We get the tools we depend upon via `npm`, the [node package manager][npm].
* We get the ionic code via `bower`, a [client-side code package manager][bower].

We have preconfigured `npm` to automatically run `bower` so we can simply do:

```
npm install
```

Behind the scenes this will also call `bower install`.  You should find that you have three new folders in your project.

* `node_modules` - contains the npm packages for the tools we need
* `bower_components` - contains the new components files
* `app/lib/*` - contains javascripts libraries

### Run the Application

The simplest way to start application is :

```
ionic serve
```

Now browse to the app at `http://localhost:8100`.



## Directory Layout

```
hook/                           --> This directory stores any Cordova Hooks that you may have.
plugins                         --> Any Cordova Plugins that you install will be saved in this folder.
resources/                      --> all
scss/                           --> Stores Ionic's SCSS file, but you can (optionally) put your own SCSS files in there too
www/                            --> This contains the meat of our Ionic application; you'll be spending most of your time in here.
  app/  --> All of your application Javascript files will be place in here.
    templates/                  --> all ionic view templates store here
    app.js                      --> main javascript file that handle your application bootstraping, configuring and runing
    controllers.js              --> all controllers defined here
    directives.js               --> all directives defined here
    filters.js                  --> all filters defined here
    services.js                 --> all services defined here
  css/                          --> Where you should store your CSS files.
  img/                          --> Where you should store any image assets.
  lib/                          --> Any external libraries will be placed in here. To start, only Ionic shows up in this folder.
  index.html                    --> This is the starting point for our application. It will load up all of the necessary JS, HTML and CSS files. Whenever you create a new Javascript or CSS file, you will need to ensure you are linking to it from the index.html file.
bower.json                    --> Used for managing your app's dependencies via the bower package management tool. By default, the Ionic Framework is the only dependency, but you can add more as needed
config-bkp-android.xml        --> This is the configuration file for Cordova. It's used for Cordova plugin management and app settings for ANDROID platform.
config-bkp-ios.xml            --> This is the configuration file for Cordova. It's used for Cordova plugin management and app settings for IOS platform.
config.xml                    --> This is the configuration file for Cordova. It's used for Cordova plugin management and app settings.
gulpfile.js                   --> This file is used for compiling SASS and other Ionic Framework specific tasks via the gulp task runner.
package.json                  --> All of your npm dependencies are stored in this file.
ionic.project                 --> This is used for the configuration of the ionic CLI tool. You can learn about some of the configuration options available [https://github.com/driftyco/ionic-cli]
```

## Updating Ionic

Previously we recommended that you merge in changes to ionic-seed into your own fork of the project.
Now that the ionic framework library code and tools are acquired through package managers (npm and
bower) you can use these tools instead to update the dependencies.

You can update the tool dependencies by running:

```
npm update
```

This will find the latest versions that match the version ranges specified in the `package.json` file.

You can update the Ionic dependencies by running:

```
bower update
```

This will find the latest versions that match the version ranges specified in the `bower.json` file.

## Contact

For more information on project please check out http://ionicframework.com

[ionicframework]: http://ionicframework.com/
[git]: http://git-scm.com/
[bower]: http://bower.io
[npm]: https://www.npmjs.org/
[node]: http://nodejs.org

## Contact

* Ali Pour Zahmatkesh ( info[at]ali-pourzahmatkesh.com ) [http://wwww.ali-pourzahmatkesh.com]
* Mohammad Reza Golabshekar ( m.golabshekar[at]gmail.com )