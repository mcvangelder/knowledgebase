# Debug with VS Code
This document will show how to setup Visual Studio Code to be able to debug react applications

## Create Launch Configuration File
To create the launch configuration file:
1. Navigate to `Run and Debug` menu (`Ctrl + Shift + D`).
2. Select `create a launch.json file`
3. Choose `Web App (Chrome)`

    A configuration as below will be displayed in the file. Be sure to update the port `8080` to `3000`
4. Click Save

## Configuration
```json
{
  "version": "0.2.0",
  "configurations": [
    {
      "type": "chrome",
      "request": "launch",
      "name": "Launch Chrome against localhost",
      "url": "http://localhost:3000",
      "webRoot": "${workspaceFolder}"
    }
  ]
}
```