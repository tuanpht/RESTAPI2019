---?color=black
@title[Title]

@snap[west headline text-white span-70]
React.js
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend


---
@title[Contents]
### Contents

@ol[](false)
- What is React.js?
- Why React.js?
- Setup
- Your First Component

---
@title[Contents]
### Contents

@ol[](false)
- **What is React.js?**
- Why React.js?
- Setup
- Your First Component


---
@title[What is React.js?]
### What is React.js?

@ul[list-bullets-black](true)
- It's a library for building @size[1.5em](user interfaces)
- React builds the UI with @size[1.5em](components)
- These components usually have changing @size[1.5em](data)
- React was created at Facebook
- It's used by Netflix, NY Times, Uber, Twitter, etc.
- Visit React.js [website](https://reactjs.org/)

@ulend

---
@title[Contents]
### Contents

@ol[](false)
- What is React.js?
- **Why React.js?**
- Setup
- Your First Component

---
@title[Why React.js?]
### Why React.js?

@ul[list-bullets-black](true)
- React is becoming very popular [*](https://insights.stackoverflow.com/survey/2018/)
- It uses a Component based architecture [*](https://twitter.com/lyit)
- React builds website UI using @size[1.5em](components)
- @size[1.5em](Components)
- @size[1.75em](Components)
- @size[2.0em](Components)
@ulend


---
@title[Contents]
### Contents

@ol[](false)
- What is React.js?
- Why React.js?
- **Setup**
- Your First Component


---
@title[React Setup]
### React.js Setup

We are going to need:
@ul[list-bullets-black](true)
- the _React Developer Tools_ browser extension
- the _Create React App_ tool 

@ulend


---
@title[React Setup]
### React Developer Tools

@ul[list-bullets-black](true)
- Install from [Chrome Webstore](https://chrome.google.com/webstore/category/extensions)
- Search for *React Developer Tools*
- It helps you:
  - identify any website you visit that uses React [*](https://www.instagram.com/?hl=en)
  - provides a React tab in the console
- Install it now!
@ulend

---
@title[React Setup]
### Create React App

@ul[list-bullets-black](true)
- Create React App creates a new React app for you
- You'll need `node` version 8 || > to install it
- Let's install it now...
@ulend

---
@title[React Setup]
### Create React App

Install Create React App

```
C:\> node -v
v8.9.4

C:\> npm install -g create-react-app
     ...

C:\>
```
@ul[list-bullets-black](true)
- Where was it installed?
- `c:\users\YOU\AppData\Roaming\npm`
- add folder to `PATH`...
@ulend

---
@title[React Setup]
### Create React App

Setup `PATH`
```
C:\> set PATH=%PATH%;c:\users\YOU\AppData\Roaming\npm

```
Test it works:
```
C:\> create-react-app
     ...
```
@ul[list-bullets-black](true)
- Let's create our first React.js app...
@ulend

---
@title[Hello React App]
### Hello React App

```
C:\> create-react-app helloreact
     ...
```
@ul[list-bullets-black](true)
- Let's run the app...
@ulend

---
@title[Hello React App]
### Hello React App

```
C:\> cd helloreact
C:\helloreact> npm start
               ...

```
@ul[list-bullets-black](true)
- Use Chrome to visit [http://localhost:3000](http://localhost:3000)
- Open the app with VS Code for a quick tour...
@ulend

---
@title[Hello React Quick Tour]
### Hello React Quick Tour

@ul[list-bullets-black](true)
- `public/index.html`
  - the `<div>`
- `src/index.js`
  - imports
  - `ReactDOM.render()`
- `src/App.js`
  - imports
  - `App` component
  - render JSX
- View the `<App>` component in React tab
@ulend

---
@title[Contents]
### Contents

@ol[](false)
- What is React.js?
- Why React.js?
- Setup
- **Your First Component**


---
@title[Your First Component]
### Your First Component

@ul[list-bullets-black](true)
- Let's create our own  @size[1.5em](React Component)
- It will just display a `<h1>` heading 
- Let's create it...
@ulend


---
@title[Your First Component]
### Your First Component

```javascript
// src/HelloWorld.js
import React from 'react';
import ReactDOM from 'react-dom'

class HelloWorld extends React.Component {
  render() {
    return (
      <h1>Hello World!</h1>
    );
  }
}
export default HelloWorld;
```
@[2](import React library)
@[2,3](import ReactDOM to render the component)
@[2,3,5,11](Our component extends from a React.Component)
@[2,3,5,11,6,10](All components MUST have a render method)
@[2,3,5,11,6,10,7,8,9](return the component element)
@[8](this is JSX)
@[12](export the component class)
@[*]()

@ul[list-bullets-black](true)
- Let's render this component to our HTML page...
@ulend

---
@title[Your First Component]
### Your First Component

```html
<!-- public/index.html -->
<!doctype html>
<html lang="en">
<head>
  <title>React App</title>
</head>
<body>
  <div id="root"></div>
</body>
</html>
```

@[8](We'll add the component here)
@[*]()

---
@title[Your First Component]
### Your First Component

```javascript
// src/index.js
import React from 'react';
import ReactDOM from 'react-dom';
import HelloWorld from './HelloWorld.js';

ReactDOM.render(<HelloWorld />, 
                document.getElementById('root'));
```

@[2,3](import React and ReactDOM)
@[2,3,4](import our new component)
@[2,3,4,6-7](render our HelloWorld component in the div)
@[*]()

@ul[list-bullets-black](true)
- View in browser 
- and examine the React console tab too
@ulend


---
@title[Exercise]
### React.js Exercise 1 – Getting Started

[@fa[external-link]](https://github.com/noucampdotorgRESTAPI2019/ReactJS/blob/master/exercises/ReactEx1.md)


---
@title[JSX]
### JSX



---?color=black
@title[Title]

@snap[west headline text-white span-70]
React.js
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend
