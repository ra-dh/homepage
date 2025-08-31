# Home page for the relationship anarchy group in The Hague
[![Build][github-build-badge]][github-build]

## Quick Start
This homepage is build using material for [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)

To build the pages and see edits live using [Docker](https://www.docker.com/):

```shell
cd docs/
make
```

Or using [Python 3](https://www.python.org/), creating and activating a _virtual environment_:

```shell
cd docs/

python3 -m venv .venv
source .venv/bin/activate

pip install -r requirements.txt
mkdocs serve

deactivate
```

Or using [UV](https://docs.astral.sh/uv/), creating and activating a _virtual environment_:

```shell
cd docs/

uv venv

uv pip install -r requirements.txt
uv run mkdocs serve
```

Navigate to [localhost:8000](http://localhost:8000/) to see the documentation.
The local documentation is automatically reloaded when changes occur.
Changes pushed to the `main` branch are automatically deployed to Github Pages.



## Updating Dependencies
Install the [`pip-check-updates`](https://pypi.org/project/pip-check-updates/) tool in a _virtual environment_ (e.g., using `pip install pip-check-updates` or `uv pip install pip-check-updates`). Usage:

```shell
cd docs/
pcu requirements.txt
```

And update the dependencies to their latest versions using:

```shell
cd docs/
pcu -u requirements.txt
```

> [!NOTE]
> Install the updated dependencies using:
>
> ```shell
> pip install -r requirements.txt
> ```
>
> Or, when using UV:
>
> ```shell
> uv pip install -r requirements.txt
> ```
