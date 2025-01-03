# Project Setup

## Clone project from GitHub Repo

First thing you should do is clone the project from the [Github Repo](https://github.com/dappuniversity/react_hardhat_template).

## Dependencies & package.json

You will want to grab all of the `package.json` dependencies from the master zip file. Copy/paste them into your project.
Copying these exact dependencies will make following along much easier in the future when updates may cause breaking changes!

```json
{
  "name": "dapp_punks",
  "version": "0.1.0",
  "private": true,
  "dependencies": {
    "@testing-library/jest-dom": "^5.16.5",
    "@testing-library/react": "^13.3.0",
    "@testing-library/user-event": "^13.5.0",
    "bootstrap": "^5.2.0",
    "react": "^18.2.0",
    "react-bootstrap": "^2.5.0",
    "react-countdown": "^2.3.2",
    "react-dom": "^18.2.0",
    "react-scripts": "5.0.1",
    "web-vitals": "^2.1.4"
  },
  "scripts": {
    "start": "react-scripts start",
    "build": "react-scripts build",
    "test": "react-scripts test",
    "eject": "react-scripts eject"
  },
  "eslintConfig": {
    "extends": ["react-app", "react-app/jest"]
  },
  "browserslist": {
    "production": [">0.2%", "not dead", "not op_mini all"],
    "development": [
      "last 1 chrome version",
      "last 1 firefox version",
      "last 1 safari version"
    ]
  },
  "devDependencies": {
    "@nomicfoundation/hardhat-toolbox": "^1.0.2",
    "hardhat": "^2.10.1"
  }
}
```

## Install the dependencies

Just having these in your `package.json` doesn't mean they are installed in **YOUR** project.
So make sure you open this _whole_ project inside your `VSCode`.
Now open your terminal in `VSCode` and run:

```bash
npm install
```

**OR**

```bash
npm i
```

`npm i` is the same and just shorter for us lazy people.
You must always install your dependencies after you clone a `GIT REPO`.

## Run a test to make sure your project is working as intended

Inside your terminal, run:

```bash
npx hardhat test
```

This will run throught the tests that are already written inside `test/Token.js`

And you can also run the website to make sure that is working with:

```bash
npm run start
```

### How to kill your running server in command line

When you run your web server, it will continue to run until you stop it or something goes wrong.
You can manually kill with:

```bash
Ctrl + C
```
