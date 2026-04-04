# GitHub CodeSpaces
In order to create a new GitHub CodeSpace with:
- python 3.13
- Conda (included by default in the Python image)
- UV (included in requirements.txt)
- Azure CLI

, please create:
- `.devcontainer` folder in the root
- the following `.devcontainer.json` file into that folder 
```json
{
  "image": "mcr.microsoft.com/devcontainers/python:3.13",
  "postCreateCommand": "pip install -r requirements.txt && curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash"
}
```
