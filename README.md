# CDK Vscode Devcontainer Example

This is a simple example of a CDK project that can be used with the VSCode Devcontainer extension.

## Prerequisites

- Docker
- VSCode
- [VSCode Devcontainer extension](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers)
- AWSCLI on your local machine

## How to use

1. Open this project in vscode

2. Install `Devcontainer extension` in vscode

3. `ctrl+shift+p` -> `Dev Containers: Open folder in Container`

4. Select the `infra` folder

5. Open terminal in vscode container

6. Run `aws sts get-caller-identity` to check if your aws credentials are working

7. Run `cdk bootstrap` and then, `cdk deploy` to deploy the stack


## Git 

if you want to commit and push the repository inside the container, you need to set your git credentials.
Run the following commands in the terminal: [ref](https://code.visualstudio.com/remote/advancedcontainers/sharing-git-credentials)

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@address"
```

and reopen the repository in the container by rebuilding the container.

- `ctrl+shift+p` -> `Dev Containers: Rebuild Container`
