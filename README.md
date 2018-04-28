# To create react project

For more info: https://github.com/gitname/react-gh-pages

Also: https://www.youtube.com/watch?v=GU-2T7k9NfI

Please use the script file attached

To use existing:

```
git clone -b master https://github.com/lightern/heavy.git
cd heavy
npm install
```

Process:

* create-react-app (npm installed app) creates a new React project
* npm (NodeJS) installs gh-pages (with that one can publish files to gh-pages branch on GitHub)
* Edit package.json file with build, gh-pages and npm deployment information
* Use "git init" -command to initialize github project (will create .github folder)
* npm run deploy to package and send the files to github

Tools used:

* npm (package manager for NodeJS backend)
* React is library for building UI
* Webpack bundles all stuf in /src folder few big files to /static folder and also adds script line to index.html (webpack is installed to project with npm)
* Babel ES5 transpiler that will transpile ES6 to ES5
* JSX enables writing "HTML" inside React
* Redux


Files:

* package.json keeps inside some information for npm, created on "npm init" (with that you can initialize the project)
* js/app.js includes the actual functions
* js/dom-loader includes the elements in the DOM
* node_modules folder includes the libraries used by Webpack
* index.js has the information of what is injected to index.html file to <div "root"> (for example)

What you need:

* github address (where the page is visible)
* domain 
