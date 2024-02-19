# Maintaining Documentation
All documentation directly relating to the APIs and specifics should use in-code API documentation wherever applicable; everything else should be documented here.

If you've been tasked with researching something, It's likely you'll need to write about it here.

## Maintanance Instructions
To add new pages simply create a new plain text file with a `.md` file extension somewhere in the `/docs` directory. Most modern IDEs will be able to parse `.md` files easily. You'll write your pages in [Markdown](https://www.markdownguide.org/cheat-sheet/) a simplified text formatting language. Any modern IDE or enhanced text editor will usually be able to highlight markdown just fine, [VSCode](https://code.visualstudio.com/) is a good reccomendation.

Once you're done simply commit your files to the repo using git, and a GitHubAction will automatically regenerate and redeploy the website for you, that's it! If you'd like to work with someone on a page but not commit to the web every push, you can create a separate branch to isolate it from the autodeployment, but this is not neccessary.

## Entirely Optional Installation of MKDocs
If you'd like to have a live preview or be able to push directly to the live web version, you'll need to install MKDocs.

Make sure you have a relatively modern version of python and the pip package manager installed, then install mkdocs using `pip install mkdocs`.

If you're on windows you may need to use `python -m` in front of your commands to get them to run with the correct permissions.

Once that's done you should be able to use all the mkdocs commands listed below or on the [official mkdocs documentation](https://www.mkdocs.org/).

## General MKDocs Documentation

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

### Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.
