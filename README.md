NAIST IEEE Student Branch Information Website
====================

Agency theme based on [Agency bootstrap theme ](https://startbootstrap.com/template-overviews/agency/)


# Run locally

If you just cloned this repository, install first the dependencies

(Optional) if you don't have bundler installed, install it first: `gem install bundler`

```bash
# move into this repository's directory after cloning
$ cd ieee-sb-naist.github.io
# isolate gems installation to only this project
$ bundle config set --local path 'vendor/bundle'
# Install requirements
$ bundle install
```

Then you can locally run this repository

```bash
$ bundle exec jekyll serve --livereload
```

## Troubleshooting

In MacOS gems' installation might fail. In that case, you might have to change the ownership of Ruby's library directories

```bash
$ sudo chown -R $(whoami) /Library/Ruby/Gems/*
```

For Apple silicon (M1, M2, etc) computers, you might need to set a build parameter for `ffi`'s gem.

```bash
# (Optional) if you already installed this repository requirements, delete them
$ rm -rf vendor/bundle
# Add build parameters for ffi's gem. These config preferences will be saved in .bundle/config
$ bundle config build.ffi --enable-libffi-alloc
# Reinstall this repository's requirements
$ bundle install
```

# Basic Content Modification

## Content edition

### Events

Events projects are defined in `/_posts`

Images are in `/img/events/`

### About

Images are in `/img/about/`

### Team

Team members and info are in `/_config.yml`

Images are in `/img/team/`

## Template layout modification

You can modify the different sections of the website in the html templates found in `/_includes/`.

They use a scripting language called 'Liquid'. You can learn the basics at their [official documentation](https://shopify.github.io/liquid/basics/introduction/) and the particular feature enhancements at [Jekyll's official documentation](https://jekyllrb.com/docs/liquid/).

# Demo

View this jekyll theme in action [here](https://y7kim.github.io/agency-jekyll-theme)

=========
For more details, read [documentation](http://jekyllrb.com/)
