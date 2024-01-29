# full-poetry-install

A Github action for doing a full, cache-enabled Poetry project installation.

Checks out your repo, installs Poetry and setups a venv, all with a cache.

## Usage
```yml
- name: Full Poetry install
  uses: emanueljg/full-poetry-install@master
  with:
    python: '3.11'
    self-cache: 'poetry-0'  # if set to str, cache poetry with this key.
```
