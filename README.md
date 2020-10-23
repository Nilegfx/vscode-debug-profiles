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
