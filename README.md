# Still in progress :sweat_smile:	   

# References
- Fullstack react the complete guide to reactjs and friends, Anthony Accomazzo & Nathaniel Murray & Ari Lerner
- React's Documentation

# Summary
- [Software install](#software-install)
- [Creating React app](#creating-react-app)
- [Modifying inital files](#tabela-de-conteudo)
- [Starting app](#instalacao)
- [Folder structure](#como-usar)
- [Design System](#testes)
- [Deploying on GitGub Pages](#tecnologias)

# Software install

## Node.js
  Download Node.js (version > 8.10) at https://nodejs.org/en/
  It's not really necessary to have Node.js installed but it will help you since Node has the package manager NPM

## Code editor
  This is up to you, I use Visual Studio Code (https://code.visualstudio.com/download) since it doesn't request much of mine computer's processor and it has the possibility to download extensions such as code formatter, snippets, intelisense and many others.

# Creating React app
  Well not a surprise here, I use the command create-react-app (created by Facebook) which is a very fast way to start you project. It's important to say that you need to have Node.js or any other Package Manager installed in your machine in order to use this command.
  
#### Code in JavaScript
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
  
#### Code in TypeScript
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
