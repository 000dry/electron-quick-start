# ELECTRON START KIT

### pre-requisites:

- install xcode via app store + open and accept terms and conditions
- install node version manager: `curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.38.0/install.sh | bash`
- verify install: `nvm -v`
- install node: `nvm install node`
- use node: `nvm use node`
- verify: `node -v && npm -v` (node should be v18)

### set up project:

- follow steps on electron docs: https://www.electronjs.org/docs/latest/tutorial/quick-start#scaffold-the-project
- add to package.json scripts block: `"start:nodemon": "nodemon --watch main.js --exec npm start"`
- install nodemon: `npm i nodemon`
- to open devtools, add the following line to your create window function: 

```js
    win.webContents.openDevTools()
```

### notifications:

- your mac may try to switch of notifications if it notices many notifications triggered by dev work, fix as below:

`System Preferences -> Notifications & Focus -> Electron` and toggle switch that says "Allow Notifications from Electron" 

