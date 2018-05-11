# Slideshow Sandbox

Note that while this repository is private (as slides repositories should be), the GitHub Pages mechanism used publishes slides publicly (from the docs folder).

The mechanism used to publish slides relies on [Slideshow (S9)](https://slideshow-s9.github.io/), a [Ruby](https://www.ruby-lang.org) gem. The published slides use a customized template leveraging [reveal.js](https://github.com/hakimel/reveal.js/).

## Publishing Slides
For publishing instructions, see [./src/](./src/)

## Environment Setup

### Install Ruby

Here are the basics. For more information, see [Installing Ruby](https://www.ruby-lang.org/en/documentation/installation/).

#### Windows

Install (latest) Ruby version from [RubyInstaller](https://rubyinstaller.org/).

#### Linux and OS X

Linux and OS X install Ruby at the OS level, but you don't want to use this install, since you'd need to `sudo` everything. Instead, it's suggested you use the [chruby](https://github.com/postmodern/chruby) Ruby version manager along with [ruby-install](https://github.com/postmodern/ruby-install) to install a Ruby version(s). On OS X, you'll want to use [homebrew](https://brew.sh/) for this.

### Install bundler

After ruby is installed, run `gem install bundler` to install the bundler gem. Now you're good to go!

