# Wiki Local Hosting
To make editing easier and more efficient, it is highly recommended to host the wiki locally. The setup process only needs to be done once. Follow the steps below to get started.

## Python Installation
MkDocs is a Python package, so the first step is to install [Python and pip](https://www.python.org/downloads/).

```sh
python --version
```

After installation, verify that Python and pip are correctly installed by running the following commands in your terminal. If the commands show the version numbers, then everything is installed correctly.

```sh
pip --version
```

## MkDocs Installation
Once Python and pip are set up, you can install MkDocs using pip. Run the following command in your terminal:

```sh
pip install mkdocs
```

Confirm successful installation by checking the MkDocs version.

```sh
mkdocs --version
```

!!! info
    For additional details, see the [MkDocs Installation Reference](https://www.mkdocs.org/user-guide/installation/#installing-mkdocs).


## Material for MkDocs Installation
This wiki uses the Material Theme for MkDocs. To install it, run the following pip command:

```sh
pip install mkdocs-material
```

!!! info
    For more information, visit the [Material for MkDocs Documentation](https://squidfunk.github.io/mkdocs-material/getting-started/)


## Running the Webpage locally
Once everything is installed, you can serve the wiki locally to preview the webpage. Navigate to the main repository folder in the terminal, and run:

```sh
mkdocs serve
```

This command starts a local server, which you can access at [localhost:8000](http://localhost:8000/) in your browser.

!!! warning
    Make sure to navigate to the main repo folder before running the `serve` command!

MkDocs includes a live-reloading server, which means any changes you make to the files will be immediately visible on the local site without the need to restart the server.

!!! info
    Additional information can be found in the [MkDocs Hosting Reference](https://squidfunk.github.io/mkdocs-material/creating-your-site/)

## Publishing
The wiki is set up to automatically rebuild and deploy on GitHub Pages whenever there is a new commit to the `master` or `main` branch. Once deployed, the wiki becomes accessible via its GitHub Pages URL.

The deployment logic is defined in the `./.github/workflows/ci.yml` file in the repository.

