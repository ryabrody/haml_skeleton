# How to use HAML without creating a Rails App
This repo is a skeleton for static pages created by writing haml instead of html.

# Setup and Usage

Install all listed gems in the Gemfile with bundler:
```bash
bundle install
```
To generate or update the index.html we use a guard watcher. More about guard-haml: https://github.com/guard/guard-haml 
Start the guard watcher with following command, this will compile the index.haml after each save to index.html.
```bash
bundle exec guard
```
To end the guard-watcher type `exit`.

Open the index.html in a browser to look at your fancy changes:
```bash
open index.html
```

If you wanna compile the .haml file without guard then just do it with haml itself:
```bash
haml index.haml index.html
```
sources:
* http://stackoverflow.com/questions/6125265/using-layouts-in-haml-files-independently-of-rails
* http://ezekielbinion.com/blog/how-to-use-haml-coffeescript-sass-without-creating-a-rails-app/
