# Editing the Website

These instructions assume a UNIX-like (OSX in particular) OS.

You should be able to get a local rendering system going to preview your
edits by following these instructions:

1. Make sure you have xcode installed with command line tools `xcodeselect --install`.
2. Use homebrew to install Ruby and gem support `brew install ruby`
3. [Install Jekyll](https://jekyllrb.com/docs/installation/)

Then you should be able to:

```bash
$ cd docs
$ bundle install
$ bundle exec jekyll serve --incremental
```

and then use the URL it gives you. It will recompile on save, but you have
to reload the browser page to see changes.

## Publishing

Do edits on the `develop` branch unless it is some kind of hot fix (in
which case you should use git flow hotfix).

The live website is auto-generated from the current `master`. So, merging
and pushing to master will update the website.
