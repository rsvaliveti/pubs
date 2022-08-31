# Radha Valiveti's Publications

BibTeX entries for  Radha Valiveti's publications. I plan to use this repository to populate the publications in my [CV][rsv-cv], as well as my personal [website][rsv-website]. As it stands, each "project" includes its own copy of the `.bib` files for my papers and patents. 

I plan to save the PDFs for my papers (when available) on my personal website. Currently, these PDF files are saved only in my Google Drive, and are not publicly accessible.

[rsv-cv]: https://github.com/rsvaliveti/cv
[rsv-website]: https://rsvaliveti.github.io/

## Adding this repo to a LaTeX paper repo

One way to add this repository to a paper repository is via the [git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules) command. Do the following in your paper repository:
```
$ git submodule add https://github.com/rsvaliveti/pubs
$ git commit -am 'added RSV pubs submodule'
$ git push origin master
```
Now if you freshly clone this repository elsewhere, you'll find an _empty_ `pubs` directory. To populate it, do:
```
$ git submodule init
$ git submodule update
```
Git submodules are tricky, and not everyone likes them, but they are one way to stay in sync. One thing to keep in mind is that you need to _be_ in the submodule subdirectory to run any git commands specific to that submodule.
