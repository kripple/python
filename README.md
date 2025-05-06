# Python

## Setup & Installation

```bash
# An extremely fast Python package and project manager, written in Rust.
# https://github.com/astral-sh/uv
curl -LsSf https://astral.sh/uv/install.sh | sh
source $HOME/.local/bin/env

uv --version # uv 0.7.2 (481d05d8d 2025-04-30)
# uv can update itself to the latest version:
# uv self update

# To install the latest Python version:
uv python install

# uv requires using a virtual environment by default
# create a virtual environment at .venv
uv venv

# Activate with:
source .venv/bin/activate

# Install a package in the new virtual environment
uv pip install Django
python -m django --version # 5.2

# Auto-generate Django project
django-admin startproject src .

# Run the dev server
# The development server automatically reloads Python code for each request as needed. You don’t need to restart the server for code changes to take effect. However, some actions like adding files don’t trigger a restart, so you’ll have to restart the server in these cases.
python manage.py runserver

# To exit a virtual environment, use the deactivate command:
deactivate
```

## Development

```bash
source $HOME/.local/bin/env
source .venv/bin/activate

# Run the dev server
python manage.py runserver

# Create a new app `polls`
python manage.py startapp polls

# View at http://127.0.0.1:8000/polls/
```
