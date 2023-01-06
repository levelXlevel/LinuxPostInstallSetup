# Linux Post Install Setup

## Problem

Anytime I install/re-install Linux on a piece of hardware (mine or someone elses) there is usually some level of post-installation configuration needed in order to make better use of the system. Rather than maintaining a stash of documents all to myself, I figured I'd lear a few new things (git, mkdocs, yml, markdown) and try to create something more accessible.

## Solution

I settled on mkdocs to handle the task of managing the documents.

## Contributing

It's my first project primarily for my own use. That said I am willing to accept feed back & commits. Not sure exactly how I want to do that, but yeah, there it is.

## Setup the project

1. Read the [MkDocs](https://www.mkdocs.org/) documentation.
1. Clone the repo.
1. Change to the project folder.
1. Create a python (3.x) environment using `python -m venv .env` or whatever method you use.
1. Activate the environment you just created:
   1. source ./.env/bin/activate
   1. source ./.env/bin/activate.fish
   1. Or whatever is the equivalent for your setup.
1. Install dependencies using `pip install -r install.txt`1.
1. Launch the mkdoc server using `mkdocs serve`1.
1. View the docs in your [browser](http://localhost:8000/)

## Edit

1. Open the project folder in your editor of choice.
1. Read the [MkDocs](https://www.mkdocs.org/) documentation.
1. Edit the document.
1. Have questions? Please re-read the [MkDocs](https://www.mkdocs.org/) documentation.

## Recommendations

- Keep it simple, the reader shouldn't need a decision tree in order to figure things out.
- Use references; Try not to recreate a modified version of a page, instead see if it makes more sense to modify the page being references.
