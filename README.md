# Node.js Express App

## _A basic starting point for your Node.js Express projects, built with Webpack._

- The build is based on vanilla JS with no specific frontend framework in mind,
- but you can definitely add the frontend framework of your choice and update configurations accordingly.
- Also, there is no particular db setup taken into mind, so you should set up the db of your choice and configure accordingly.

<br/>

### This project assumes you will use

- JavaScript
- Express.js server
- The rest (frontend framework, db, etc.) is left for the user to freely configure

<br/>

## Getting Started

Initiate your project by running below command in the directory of your choice:
<br/>
(Replace 'my-app' with your choice of project name)

```
npx nodejs-express-app my-app
```

- This will:
  - download all necessary files and folders,
  - generate package.json
  - initialize git

Then, make sure to install dependencies:

```
npm install
```

To start the development server, run:

```
npm start
```

- This will run two different scripts:
  - `webpack serve --config webpack.dev.js`
  - `nodemon server/server.js`
- Development server has been designed to run two separate servers:
  - Webpack Dev Server for frontend (at PORT 3031)
  - Express Server for backend APIs (at PORT 8085)
- Other scripts are also included for starting the server (e.g. `npm run start:dev2`, which uses `webpack-dev-middleware`), but hot reload does not work with these.
- Using `npm start` is recommended.
- To adjust ports and other settings/logic, please configure accordingly.

To build your project for production, run:

```
npm run build
```

<br/>

## Notes on Configuration

If you decide to change certain property names and values in `package.json` (e.g. `main, html, fallback, favicon, etc.`) or change the name/location of the main project file (which is set to `src/index.js`), please make sure to update the relevant configurations in webpack accordingly.

<br/>

## Requirements:

(as of 2021.08.18)

- _LTS versions of node & npm_
  - node v.14.17.5
  - npm v.6.14.14
  - Other versions of node & npm have not yet been tested other than v.15.4.0, which is known to fail.
  - Using LTS version is recommended.

<br/>

## Current Known Issues

(as of 2021.08.18):

- _Install fails on node v.15.4.0_
  - Other variations of v15 have not been tested

<br/>

## Issues

If you find any new bugs/errors, please file issues at:
https://github.com/pdl39/nodejs-express-app/issues

<br/>

## Thanks!

## Happy Coding :)
