Code for Portland
=================

[![Build Status](https://travis-ci.org/CodeForPortland/codeforportland.github.io.svg?branch=master)](https://travis-ci.org/CodeForPortland/codeforportland.github.io)

Repo for the homepage of Code for Portland, a Code for America brigade based in Portland, Oregon.

Usage
-----

### Build Prerequisites

- [Git](http://git-scm.com/)
- [NodeJS](http://nodejs.org) (v0.10.26+ and NPM v1.4.4+)
  - [Bower](http://bower.io/) with `npm install -g bower` (v1.3.2+)
  - [Grunt](http://gruntjs.com) with `npm install -g grunt-cli`
- [Ruby](https://www.ruby-lang.org/en/) (Follow this [Guide](https://help.github.com/articles/using-jekyll-with-pages))
  - [Bundler](http://bundler.io) with `gem install bundler`
    - [Jekyll](http://jekyllrb.com) with `bundle install` in the working directory

### Building the Site

> **Warning:** The site's build scripts will overwrite anything in the `_dev` or `_site` directories, without any warning whatsoever. Similarly, the `assets/js` and `assets/css` directories should be considered forfeit as well: the SCSS and JS compilation scripts overwrite stuff in there!

Before you get started, get your prerequisites installed:

```cli
# With a working npm install
npm install -g grunt-cli
npm install -g bower

# With a working gem install
gem install bundler

cd <project_directory>
npm install
bower install
bundle install
```

There are two build targets: `dev`, and `deploy`.

#### Running the Development Server

The provided Gruntfile gives you a local copy of the site, running on `http://localhost:8002`. Run 

```
grunt dev
``` 

to build the dev site, and serve it on that address. Changes made to any relevant files will trigger a rebuild and livereload in any browsers you have open to the site.

#### Building the Production Site

The production site is build by issuing a `grunt deploy`. Then, commit your changes to the `gh-pages` branch, or your `master` branch if this is your github.io page.

> **Note:** Although Github's Jekyll will be building your site, you still need to run the `grunt deploy` script to generate minimized assets for your site!

## Specifications

- Photos for the main page should be 3840 × 1200 for Retina displays, and 1920 × 600

The MIT License (MIT)
---------------------

Copyright (c) 2014 Nathan Wittstock

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

