# To create react project

For more info: https://github.com/gitname/react-gh-pages

Also: https://www.youtube.com/watch?v=GU-2T7k9NfI

Please use the script file attached

## If having compile problems with error message:

"Error: ENOSPC: no space left on device, watch '/home/user/react/projectname/public'"

With Arch linux:
```
echo fs.inotify.max_user_watches=524288 | sudo tee /etc/sysctl.d/40-max-user-watches.conf && sudo sysctl --system
```
For other os:s and more info: https://github.com/guard/listen/wiki/Increasing-the-amount-of-inotify-watchers


## To use existing:

```
git clone -b master https://github.com/lightern/heavy.git
cd heavy
npm install
```

## Process:

* create-react-app (npm installed app) creates a new React project
* npm (NodeJS) installs gh-pages (with that one can publish files to gh-pages branch on GitHub)
* Edit package.json file with build, gh-pages and npm deployment information
* Use "git init" -command to initialize github project (will create .github folder)
* npm run deploy to package and send the files to github

## Tools used:

* npm (package manager for NodeJS backend)
* React is library for building UI
* Webpack bundles all stuf in /src folder few big files to /static folder and also adds script line to index.html (webpack is installed to project with npm)
* Babel ES5 transpiler that will transpile ES6 to ES5
* JSX enables writing "HTML" inside React
* Redux
* react-boostrap includes all react-boostrap components (installed via npm)


## Files:

* package.json keeps inside some information for npm, created on "npm init" (with that you can initialize the project)
* js/app.js includes the actual functions
* js/dom-loader includes the elements in the DOM
* node_modules folder includes the libraries used by Webpack
* index.js has the information of what is injected to index.html file to <div "root"> (for example)

## What you need:

* github address (where the page is visible)
* domain 

## When creating PostreSQL database:
 * First line as SERIAL and primary key
 * remember to run in phppgadmin (gives permission for automatic id numbering): GRANT USAGE, SELECT ON SEQUENCE companies_<idcolumn>_seq TO <database_username>
 * sudo ssh <hostingusername>@<hostingaddress> -p<hostingport, for example 21098> -L 5432:127.0.0.1:5432 -N
