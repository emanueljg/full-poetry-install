# full-poetry-install

A Github action for doing a full, cache-enabled Poetry project installation.

Checks out your repo, installs Poetry and setups a venv, all with a cache.
Wrapper around [setup-python](https://github.com/actions/setup-python) and [install-poetry](https://github.com/snok/install-poetry), basically executing [these](https://github.com/snok/install-poetry?tab=readme-ov-file#testing) steps.

## Usage
```yml
- name: Full Poetry install
  uses: emanueljg/full-poetry-install@v1
  with:
    python: '3.11'
    self-cache: 'poetry-0'  # if set to str, cache poetry with this key.
```
