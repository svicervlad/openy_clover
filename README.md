# Maintaining the theme.

##1. Install Yarn

###macOS

####Homebrew

You can install Yarn through the Homebrew package manager. 
This will also install Node.js if it is not already installed.

`brew install yarn`

If you use nvm or similar, you should exclude installing Node.js 
so that nvm’s version of Node.js is used.

`brew install yarn --without-node`

####MacPorts

You can install Yarn through MacPorts. 
This will also install Node.js if it is not already installed.

`sudo port install yarn`

###Debian / Ubuntu

https://yarnpkg.com/lang/en/docs/install/#debian-stable

###Windows
https://yarnpkg.com/lang/en/docs/install/#windows-stable

##2. Go to the theme's folder

`yarn install`

##3. Compile all assets

`grunt build`

##4. Start watching all assets (for development)

`./node_modules/grunt/bin/grunt watch`

# Install with composer:

add to composer.json your openy project in section "repositories":
```json
{
    "type": "package",
    "package": {
        "name": "svicervlad/openy_clover",
        "version": "1.0",
        "type": "drupal-theme",
        "dist": {
            "url": "https://github.com/svicervlad/openy_clover/archive/composer_support.zip",
            "type": "zip"
        }
    }
 },
```