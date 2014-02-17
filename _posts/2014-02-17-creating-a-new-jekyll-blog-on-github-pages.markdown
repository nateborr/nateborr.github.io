---
title: "Creating a new Jekyll blog on GitHub Pages"
layout: post
date: 2014-02-17 14:30:00
---

I've just spun up a new Jekyll site on GitHub pages, which is straightforward as advertised. The installation process is clearly documented between the two sides:

* GitHub: [Using Jekyll with Pages](https://help.github.com/articles/using-jekyll-with-pages)
* Jekyll: [GitHub Pages](http://jekyllrb.com/docs/github-pages/)

If you're already set up with Ruby and Bundler on your local machine and a GitHub user account whose Pages you want to deploy to, creating and deploying a boilerplate site as I did takes very few steps:

1. On GitHub, create a new repo named after the Pages URL for the user account, for example "nateborr.github.io".
2. Clone the new repo to your local machine. `cd` into its root directory.
3. Create a Gemfile with `bundle init` and add to it: `gem 'github-pages'`
4. `bundle install`.
5. Create a new Jekyll site in the existing root directory of the repo: `bundle exec jekyll new . --force`
6. Commit all changes to the master branch and push to GitHub.
