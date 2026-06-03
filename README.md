# Boas Companion

This repository contains companion notebooks for M. L. Boas, *Mathematical Methods in the Physical Sciences*, 3rd ed., Wiley, 2005.

The project is intended to collect original solution writeups, section summaries, computational checks, and code for reproducing plots or numerical examples in Jupyter notebooks.

## Status

Chapter 1 sections 1.1 through 1.16 are available as notebooks. Sections 1.1 through 1.13 have been checked; sections 1.14 through 1.16 are draft material and may still need verification, revision, or additional computational checks.

## Contents

- `ch01/`: section-specific solution notebooks for Chapter 1, named `sec01.ipynb` through `sec16.ipynb`.
- `ch04/`: section-specific solution notebooks for Chapter 4, currently `sec01.ipynb`.
- `compose.yaml`: Docker Compose service for running JupyterLab.
- `.env.example`: example local notebook port and token settings.
- `img/`: supporting images used by this README and companion notebooks.
- `LICENSES/`: full license texts for original prose and source code.

## Running Notebooks

The easiest way to run the notebooks is with Docker Compose. The notebook service uses `quay.io/jupyter/scipy-notebook:python-3.13.13`.

Create a local `.env` file from the example:

```sh
cp .env.example .env
```

Edit `.env` if needed:

```env
NOTEBOOK_PORT=8888
NOTEBOOK_TOKEN=boas
```

Start JupyterLab:

```sh
docker compose up
```

Open any Chapter 1 notebook. For example, Section 13 is:

```text
http://127.0.0.1:8888/lab/tree/ch01/sec13.ipynb?token=boas
```

If you change `NOTEBOOK_PORT` or `NOTEBOOK_TOKEN`, update the URL accordingly.

## Development Setup

If you plan to commit changes to this repository, run this once after cloning. This keeps notebook diffs cleaner and runs the project's checks before each commit:

```sh
uv tool install nbdev pre-commit
nbdev_install_hooks
pre-commit install
```

## Source

![Alt text: Book cover of Mathematical Methods in the Physical Sciences, third edition, by Mary L. Boas, with a vector field diagram on a magenta and blue background.
](img/cover.jpg)

M. L. Boas, *Mathematical Methods in the Physical Sciences*, 3rd ed. Hoboken, NJ: Wiley, 2005.

- [Publisher page](https://www.wiley.com/en-us/Mathematical+Methods+in+the+Physical+Sciences%2C+3rd+Edition-p-9781118048887)

## Copyright Notice

This is an independent companion project. It is not affiliated with, endorsed by, or sponsored by Wiley.

The textbook, problem statements, figures, tables, cover images, and any other Wiley-owned material are not licensed by this repository. They remain the property of their respective copyright holders.

To keep the repository focused on original work, prefer references by section and problem number instead of reproducing full problem statements from the book.

## License

Unless otherwise noted:

- Original explanatory text, summaries, and solution writeups are licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License. See [LICENSES/CC-BY-NC-SA-4.0.txt](LICENSES/CC-BY-NC-SA-4.0.txt).
- Source code, including plotting and computational scripts, is licensed under the MIT License. See [LICENSES/MIT.txt](LICENSES/MIT.txt).

Files containing third-party material, including textbook cover images, are excluded from these licenses unless an explicit notice says otherwise.
