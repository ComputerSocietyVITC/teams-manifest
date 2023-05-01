# Teams Manifest 
<hr/>

This repository contains the files for the [Teams App](https://vstudent.ieeecsvitc.com) that has been deployed to the teams! Refer to the following guide
to understand how to work with it!

## Directory Structure
```
├── package.json
├── templates
│   ├── appPackage
│   │   ├── manifest.template.json
│   │   └── resources
│   │       ├── color.png
│   │       ├── outline.png
│   │       └── purple-logo.png
│   └── azure
│       ├── config.bicep
│       ├── main.bicep
│       ├── provision
│       │   ├── azureStorageTab.bicep
│       │   └── identity.bicep
│       ├── provision.bicep
│       └── teamsFx
```
Now, You don't need the NPM package if you're using the [extension](https://marketplace.visualstudio.com/items?itemName=TeamsDevApp.ms-teams-vscode-extension). The CLI
is for CI/CD purposes or if you use another editor like Vim, Emacs, etc.

The bicep files set azure up! and Honestly you don't need them!

Important files:
- [manifest.template.json](./templates/appPackage/manifest.template.json)
- [.fx](./fx)

## How to modify

Go to .fx and modify the [manifest file](.fx/states/state.dev.json) which will have the key details
