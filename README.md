# Knights on wires Jekyll proejct

This is the base repository used to create feeds, posts and links to the
bi-weekly Knights on wires podcast.

## Cloning and installing

Clone this repo using:

```
git clone --recurse-submodules git@github.com:Knights-on-wires/knights-on-wires-source.git
```

After that make sure you have Ruby (the specific version is specified in
`.too-versions`)  installed using either asdf, rvm or rbenv.

with that done execute:

```
gem install bundler # only needed on the first run
bundle install
```

you can then start a development server with:

```
bundle exec jekyll serve
```

and you can build the `_site` directory with 

```
bundle exec jekyll build
```

Make sure to commit the contents of the `_site` directory separately (it is a git
sub-module), and then push those changes up to build the production website.

Warning: `jekyll serve` generates debug versions of the website in the same
`_site` directory.
