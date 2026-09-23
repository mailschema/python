# Contributing

This repository publishes the Python package for MailSchema. The protocol schemas are maintained in [`mailschema/mailschema`](https://github.com/mailschema/mailschema); Python-specific API, CLI and packaging changes belong here and must remain compatible with those canonical files.

Run the package checks before opening a pull request:

```sh
python -m pip install -e .
python -m unittest discover -s tests -v
python -m build
python -m twine check dist/*
```

Changes to MAP behavior, shared schemas or Registry records should begin in the [main project repository](https://github.com/mailschema/mailschema/blob/main/CONTRIBUTING.md).

