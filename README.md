# Five Minute React Starter

in under 5 minutes create a lightweight react starter app from scratch

## dependencies

```
npm and node
```

## create app and init package.json from cli

```
- from cli open new dir: mkdir <app-name>
- change directory into root: cd <app-name>
- create package.json: npm init -y
- create .gitignore: touch .gitignore
```

## edit .gitignore 

open in vscode, and include: 

```
node_modules
dist/
.DS_Store
.vscode/
.cache/
.env
```

## install dependencies 

```
- install react and react-dom: npm i react react-dom
- install parcel: npm i -D parcel-bundler
```

## create hello world

```
- create src directory, in root: mkdir src
- change directory into src dir: cd src
- create root html file, in src: touch index.html
- create top level component, in src: touch App.js
- create stylesheet, in src: touch style.css
```

in file index.html, include:

```
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <meta http-equiv="X-UA-Compatible" content="ie=edge" />
    <title>react starter</title>
    <link rel="stylesheet" href="./style.css" />
  </head>
  <body>
    <div id="root">root element</div>
    <script src="./App.js"></script>
  </body>
</html>
```

in file App.js, include:

```
import React from "react";
import { render } from "react-dom";

const App = () => {
  return (
    <div>
      <h1>five minute react starter</h1>
    </div>
  );
};

render(<App />, document.getElementById("root"));
```

in file style.css, include:

```
h1 {
  color: #008080;
}
```
## build and run app

in package.json, within the scripts object, include: 

```
"dev": "parcel src/index.html"
```

cli build and run script execution

```
- in root: npm run dev
- in browser of choice, navigate to http://localhost:1234 
```

