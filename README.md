# envES6
This environment was created to have everything ready to start coding in ES6 without having compatibility problems with older browsers

# Installations

1. NodeJS: https://nodejs.org/en/
2. Yarn: https://classic.yarnpkg.com/en/docs/install/#windows-stable

P.S: After installing verify the installation with "node -v" and "yarn -v", via terminal

# Steps

* run **yarn init** to create the package.son file in the desired folder
* configure babel by running **yarn add @babel/cli** (inside the node's terminal).This command will let us work with the babel command line interface (basically it allows us to use yarn and other commands)
* run **yarn add @babel/preset-env** (inside the node's terminal)
* create the **.gitignore** file and type node_modules/ inside it, so that it doesn't get too heavy when you go up to github
* create the **.babelrc** file and put "@babel/preset-env" in it, which serves to understand the environment in which we are working and convert to the browser so that it understands
```
{
    "presets": ["@babel/preset-env"]
}
```
* run **yarn add @babel/core**
* create the path **src/js/main.js**
* on package.json, type it:
```
{
    "scripts": {
        "dev": "babel ./src/js/main.js -o ./bundle.js -w"
    }
}
```
With that, let's take what is written in “main.js” and convert it to a file called “bundle.js” (if there is an error, you can try to create the bundle file manually)

And then, after that, just program normally in the main, everything comes out in the bundle :D

P.S: to run the js script, type it "yarn dev" on node's terminal

Credits: https://medium.com/@matheusmaia_6280/configura%C3%A7%C3%A3o-de-ambiente-javascript-es6-fac281f05cca