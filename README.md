# vscode-debug-profiles

a list of vscode debug profiles which I keep using from time to time

## Debugging babel-node

```json
{
    "cwd":"${workspaceFolder}",
    "type": "node",
    "request": "launch",
    "name": "babel-node debug",
    "runtimeExecutable": "${workspaceFolder}/node_modules/.bin/babel-node",
    "program": "${file}",
    "console": "integratedTerminal",
    "runtimeArgs": ["--nolazy"]
}
```

## Debugging babel-node with nodemon
```json
{
      "type": "node",
      "request": "launch",
      "name": "Nodemon",
      "runtimeExecutable": "nodemon",
      "args": ["${workspaceFolder}/backend/index.js"],
      "restart": true,
      "protocol": "inspector",
      "stopOnEntry": false,
      "runtimeArgs": ["--nolazy"],
      "sourceMaps": true,
      "console": "integratedTerminal"
    }
```
