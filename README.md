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
