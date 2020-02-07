# create-react-extension

##　Quick Overview

```sh
npx create-react-app create-react-extension --scripts-version react-browser-extension-scripts --template browser-extension

cd create-react-extension
yarn start
```

### Yarn

```sh
yarn create react-app my-browser-extension --scripts-version react-browser-extension-scripts --template browser-extension
```

_[`yarn create <starter-kit-package>`](https://yarnpkg.com/lang/en/docs/cli/create/) is available in Yarn 0.25+_

It will create a directory called `my-browser-extension` inside the current folder.<br>
Inside that directory, it will generate the initial project structure and install the transitive dependencies:

```
my-browser-extension
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── public
│   ├── img
│   │   ├── icon-16.png
│   │   ├── icon-48.png
│   │   ├── icon-128.png
│   ├── popup.html
│   └── manifest.json
└── src
    ├── background
    │   ├── index.js
    ├── contentScripts
    │   ├── index.js
    ├── App.css
    ├── App.js
    ├── App.test.js
    ├── index.css
    ├── index.js
    ├── logo.svg
```

No configuration or complicated folder structures, only the files you need to build your extension.<br>
Once the installation is done, you can open your project folder:

```sh
cd my-browser-extension
```

## create-react-extension　vs. create-react-app

### package.json

```js
"dependencies": {
    "react-scripts": "3.3.1"  改為　"react-browser-extension-scripts": "3.3.1",
```

### src

src 新增了　background.js　和　contentScript.js

src\background\index.js
src\contentScript\index.js

### public

public\index.html 改為　public\popup.html
manifest.json 改為 chrome [Manifest File Format](https://developer.chrome.com/extensions/manifest)

## References

VasilyShelkov/[create-react-extension](https://github.com/VasilyShelkov/create-react-extension)  

