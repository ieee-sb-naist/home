Agency Jekyll theme
====================

Agency theme based on [Agency bootstrap theme ](https://startbootstrap.com/template-overviews/agency/)


# Run locally

If you just cloned this repository, install first the dependencies

(Optional) if you don't have bundler installed, install it first: `gem install bundler`

`$ bundle config set --local path 'vendor/bundle' # isolate gems installation for this project`
`$ bundle install`

Then you can run locally this repository

`$ bundle exec jekyll serve --livereload`

## Troubleshooting

In MacOS gems installation might fail. In that case, you might have to change the ownership of Ruby's library directories

`$ sudo chown -R $(whoami) /Library/Ruby/Gems/*`

For M1 or M2 mac computers, you might need to set a build parameter for ffi. If you already installed ffi, please uninstall it first (remove the bundle directory `rm -rf vendor/bundle`).

`$ bundle config build.ffi --enable-libffi-alloc`

Then reinstall dependencies

`$ bundle install`

# How to use

###Events 

Events projects are in '/_posts'

Images are in '/img/events'

###About

Images are in '/img/about/'

###Team

Team members and info are in '_config.yml'

Images are in '/img/team/'


# Demo

View this jekyll theme in action [here](https://y7kim.github.io/agency-jekyll-theme)

=========
For more details, read [documentation](http://jekyllrb.com/)
