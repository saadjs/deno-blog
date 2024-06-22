---
title: How to create Python virtual environment
publish_date: 2023-01-09
---

## Creating a virtual environment

1. From project directory run the below command to create `virualenv`:

```sh
python3 -m venv env
```

2. Activate the `virtualenv` using:

```sh
source env/bin/activate
```

3. Confirm if the virtual environment is active:

```sh
which python
```

4. To leave virtual environment:

```
deactivate
```

## Installing a Package:

Example:

```sh
python3 -m pip install requests
```

For more info:
[Installing packages using pip and virtual environments](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/)
