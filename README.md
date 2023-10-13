# Lambda build environment configurator

A github action which will help to configure the pipeline's environment and simplify managing of another pipelines by combining in one place a set of required actions.

## How to use:

### Example 1: Basic setup, no arguments needed


```yml
name: Configure environment
uses: propertylift/github.action.lambda-env-config@latest
with:
  botSshKey: ${{ secrets.BOT_SSH_KEY }}
  githubToken: ${{ secrets.GITHUB_TOKEN }}
```


## Inputs:

| Parameter Name                     | Description | Required | Default |
|------------------------------------|-------------|----------|---------|
| ansiblePythonInterpreter           | Location of python interpreter | No | /opt/pipx/venvs/ansible-core/bin/python |
| botSshKey                          | BOT's SSH key used for iteract with GitHub | Yes | - |
| githubToken                        | GITHUB_TOKEN | Yes | - |

