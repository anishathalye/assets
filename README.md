# Assets

This repository contains assets such as images and gifs that are used in my
other GitHub projects' READMEs such as
[periscope](https://github.com/anishathalye/periscope).

Often, GitHub projects place these assets in the `master` branch of the
repository itself, but this increases the `git clone` size for everyone who
clones the repo, and moreover, the assets cannot be removed from the Git
history of the main project without rewriting history, so the clone size is
permanently inflated.

Some of my projects used to keep assets in a separate `assets` branch, so at
least the large binary assets were not a part of the history of the `master`
branch, but a `git clone` still downloads all branches, so this was not ideal.

Now, all of my personal projects keep their assets in this separate repository.
