# Lambda build environment configurator

A github action to simply configure the pipeline's environment and simplify managing of whole processes.

## How to use:

### Example 1: Basic setup, no arguments needed


```yml
name: Configure environment
uses: propertylift/github.action.lambda-env-config@latest
with:
  BOT_SSH_KEY: ${{ secrets.BOT_SSH_KEY }}
  GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```


## Inputs:

| Parameter Name                     | Description | Required | Default |
|------------------------------------|-------------|----------|---------|
| ANSIBLE_PYTHON_INTERPRETER         | Location of python interpreter | No | /opt/pipx/venvs/ansible-core/bin/python |
| BOT_SSH_KEY                        | BOT's SSH key used for iteract with GitHub | Yes | - |
| GITHUB_TOKEN                       | GITHUB_TOKEN | Yes | - |

