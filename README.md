# Still in progress :sweat_smile:	   

# References
- Fullstack react the complete guide to reactjs and friends, Anthony Accomazzo & Nathaniel Murray & Ari Lerner
- React's Documentation

# Summary
- [Software install](#software-install)
- [Creating React app](#creating-react-app)
- [Modifying initial files](#modifying-initial-files)
- [Starting app](#instalacao)
- [Folder structure](#como-usar)
- [Design System](#testes)
- [Deploying on GitHub Pages](#tecnologias)

# Software install

## Node.js
  Download Node.js (version > 8.10) at https://nodejs.org/en/
  It's not really necessary to have Node.js installed but it will help you since Node has the package manager NPM

## Code editor
  This is up to you, I use Visual Studio Code (https://code.visualstudio.com/download) since it doesn't request much of mine computer's processor and it has the possibility to download extensions such as code formatter, snippets, intelisense and many others.

# Creating React app
  Well not a surprise here, I use the command create-react-app (created by Facebook) which is a very fast way to start you project. It's important to say that you need to have Node.js or any other Package Manager installed in your machine in order to use this command.
  
### Code in JavaScript
  This command will create Javascript files to your project. Open your terminal and then write one of the following commands 
```
npx create-react-app *project-name*
```
```
npm init react-app *project-name*
```
```
yarn create react-app *project-name*
```
*Example: npx create-react-app my-test-project*
  
### Code in TypeScript
  This command will create Typescript files to your project. Open your terminal and then write one of the following commands 
```
npx create-react-app *project-name* --template typescript
```
```
npm init react-app *project-name* --template typescript
```
```
yarn create react-app *project-name* --template typescript
```
*Example: npx create-react-app my-test-project* --template typescript

# Modifying Inital Files

### App.test.js | setupTests.js
Well we don't really need those files so you can delete them. BUT if you are looking for developing unit tests in your application (which I recommend) those files are important because App.test.js contains an sample of unit test for the component App and you will be able to use it as a model for the other component's unit test files and setupTests.js will import to the whole app the Jest library.
Basically the command of creating the app comes with Jest and React Testing Library which are libraries that will identify your application's components and provide unit test functions (React Testing Library) and run your test files and gives you an feedback (Jest).
