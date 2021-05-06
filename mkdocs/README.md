# Foundries.io Documentation

microPlatform documentation source for https://docs.foundries.io

# Development Environment

There are 3 ways to get started developing this documentation. Each method
provides `mkdocs` with various plugins as defined in `requirements.txt`

## Nix

Clone this repository and run `nix-shell` at the root.

1. `git clone https://github.com/foundriesio/docs/`
2. `cd docs/`
3. `nix-shell`

Then run `mkdocs serve` or use the other tools provided in this environment.

## Docker

Clone this repository and run a container on the root.

Replace `<your-git-directory>` with the path to this git repository as you have
cloned it.

1. `git clone https://github.com/foundriesio/docs/`
2. `cd docs/`
3. `docker run -v <your-git-directory>:/git matthewcroughan/mkdocs-foundries-env`

## Virtualenv

Ensure you have `python3` and `python3-virtualenv` installed. 

1. `git clone https://github.com/foundriesio/docs/`
2. `cd docs/`
3. Run the following:

```bash
$ virtualenv -p /usr/bin/python3 venv
$ . ./venv/bin/activate
$ pip install -r requirements.txt
```

Then run `mkdocs serve`

