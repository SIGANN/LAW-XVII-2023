# LAW-XVII-2023
The 17th Linguistic Annotation Workshop

This is the `main` branch; it contains sources for building the website.
The [website](https://sigann.github.io/LAW-XVII-2023) itself lives on the `gh-pages` branch.
To deploy changes:

    $ git checkout master
    # ...make, commit, and push changes...
    $ python3 build.py deploy
    $ git checkout gh-pages
    $ mv deploy/* .
    $ rmdir deploy
    $ git commit -a -m "deploy changes"
    $ git push


NB: Only edit the files under `pages/`, since these are the ones used by the build script. Any HTML files in the repository root will be overwritten on deployment.
