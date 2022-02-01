# About
Hello and welcome! This is a document that I like to follow when creating React App, I tried to write less and be more direct on each topic. 

Hope this document can help you developing you app :grinning:

# Summary
- [Software install](#software-install)
- [Creating React app](#creating-react-app)
- [Modifying initial files](#modifying-initial-files)
- [Folder structure](#folder-structure)
- [Design System](#design-system)

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

# Modifying initial files

### App.test.js
Probably your unit tests will be develop in the other component files, so you can remove this one unless you want to use this as a model for your others unit test files.

### SetupTests.js
Well we don't really need those files so you can delete them. BUT if you are looking for developing unit tests in your application (which I recommend) this file is important because setupTests.js will import to the whole app the Jest library.

Basically the command of creating the app, as seen above, comes with Jest and React Testing Library which are libraries that will identify your application's components and provide unit test functions (React Testing Library) and run your test files and gives you an feedback (Jest).

### reportWebVitals.js
Report web vitals is a tool that will measure your app's performance with metrics that focus on user experience, you can check it out the metrics here https://create-react-app.dev/docs/measuring-performance/

# Folder structure
Well for me folder structure is a concept, it's how you want your project to be organized in a way that when you project grows it will have a bunch of files agrouped by a common characteristic.

I guess the first and most common folder structure is separating components from pages, considering components being a single form for example a button, input text, text area, anyway anything that can only exist on a singular form generally it's a HTML element and the pages are the combination of these components and other pages as well.

    ├── src
    │   ├── Components
    │   ├── Pages

Ok, so what we have so far is a very basic folder structure but your project might have others characteristics, for example it could have API requests, authentications services, auxiliary functions, even might want to create an different folder for styling. Anyway, I highly recommend google the most used folder structure available but I'll leave below a more complete version of mine's:

    ├── src
    │   ├── Assets
    │   ├── Components
    │   ├── Pages
    │   ├── Services
    │   ├── Helpers
    │   ├── Hooks
    │   ├── Redux

# Design system
Well I actually read this from the book "Fullstack react the complete guide to reactjs and friends" and I found it very helpful for me and I think it could help you as well. Below we have the steps taken from the book with a few modifications that we could take in order to create a more robust system.

1. Break the app into pages
3. Break the pages into components
5. Build a static version of the app
7. Determine what should be stateful
8. Determine in which component each piece of state should live
9. Hard-code initial state
10. Add inverse data flow
11. Add server communication

Since this is a guide of how to start your project I would recommend to treat this as guide, in other words, don't be too strict to it if it doesn't work on your project. 

# References
- Fullstack react the complete guide to reactjs and friends, Anthony Accomazzo & Nathaniel Murray & Ari Lerner
- React's documentation
