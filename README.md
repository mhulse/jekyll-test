# Jekyll Boiler

**Bare bones Jekyll example site using GitHub’s “pages” gem.**

## Jekyll

First, read: [Using Jekyll with Pages](https://help.github.com/articles/using-jekyll-with-pages).

Install [Ruby, Bundler and Jekyll](https://help.github.com/articles/using-jekyll-with-pages#installing-jekyll).

You’ll probably want to install [`RVM`](http://rvm.io/) too. If it’s of any help, I have some related notes [here](https://github.com/registerguard/registerguard.github.io/wiki/Ruby-tips).

Note that this repo is a [“Project Page”](https://help.github.com/articles/using-jekyll-with-pages#using-jekyll), which means I need to create a `gh-pages` branch for this to work:

> Every GitHub Page is run through Jekyll when you push content to a specially named branch within your repository. For User Pages, use the master branch in your username.github.io repository. For Project Pages, use the gh-pages branch in your project's repository. Because a normal HTML site is also a valid Jekyll site, you don't have to do anything special to keep your standard HTML files unchanged. Jekyll has [thorough documentation](http://jekyllrb.com/docs/home/) that covers its features and usage. Simply start committing Jekyll formatted files and you'll be using Jekyll in no time.

Install missing gems:

```bash
$ cd repo/
$ bundle install
```

Or, update gems:

```
$ bundle update
```

Execute jekyll and serve:

```bash
$ bundle exec jekyll serve --baseurl ''
```

View drafts:

```bash
$ bundle exec jekyll serve --drafts --baseurl ''
```

View your locally-hosted site at <http://localhost:4000>.

## Bower

Optionally, you can use [Bower](http://bower.io/) to install/manage front-end dependencies.

First, install the Bower [packages](package.json) (assuming you already have [`npm`](https://www.npmjs.org/) installed):

```bash
$ npm install
```

Next, edit [`bower.json`](bower.json) and define desired dependency information (for documentation, read [this](http://bower.io/) and [this](https://github.com/blittle/bower-installer)).

Finally, install or update Bower dependencies:

```bash
$ npm run bower-installer
```

That’s it!

**Note:** The `gh-pages` gem does not support Bower; it’s up to you to manually update these front-end dependencies, every once in a while (when appropriate), via the command line on your local/development machine.

## Links:

* [Repository metadata on GitHub Pages](https://help.github.com/articles/repository-metadata-on-github-pages)
* [GitHub Cheat Sheet](https://github.com/tiimgreen/github-cheat-sheet)
* [Emoji cheat sheet](http://www.emoji-cheat-sheet.com/)
* [Liquid for Designers](https://github.com/Shopify/liquid/wiki/Liquid-for-Designers)
* [Using Jekyll Plugins with GitHub Pages](https://help.github.com/articles/using-jekyll-plugins-with-github-pages/)
* [Deploying Jekyll to GitHub Pages](http://jekyllrb.com/docs/github-pages/#deploying-jekyll-to-github-pages)
