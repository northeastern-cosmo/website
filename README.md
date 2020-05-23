# NU CoSMO

This repo serves as the homepage for Northeastern University's CS Mentoring Club (CoSMO).

## Usage

This site uses the static site generator `Jekyll`. Please install it in order to develop this website.

Jekyll works by taking a template that you write and generating HTML and CSS from it. If you're trying to modify the site,
you'll want to start at the root level files:
  - index.html
  - eboard.html
  - mentors.html
  - contact.html

You'll notice they contain lines like `{% include mentors.html %}`. That line imports sections of the site from the `_includes` directory.
You'll likely find what you need to change in there. `_includes` may in turn access yaml data files in `_data`. Finally, to change CSS,
look at the `assets` folder.

After editing these files, run the Jekyll command to generate the site (e.g. `jekyll serve`). You'll be able to navigate to a local version
of the new website in your browser, likely at `localhost:4000`.

### Mac Setup

[Jekyll](https://jekyllrb.com/) is a Ruby gem.  Different macOS versions ship with different versions of Ruby, so to be safe just install [homebrew's](brew.sh) Ruby. 

```bash

# Pull repo
git clone git@github.com:northeastern-cosmo/northeastern-cosmo.github.io.git
cd northeastern-cosmo.github.io

# If you don't already have homebrew installed, get it. (MUST HAVE for macOS info at http://brew.sh)
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"

# Install newer (brew's) version of Ruby
brew install ruby

# Add brew's Ruby to your path
# Note: Assumes your `echo $SHELL` == /bin/zsh. If your shell is bash, replace with ~/.bashrc
echo 'export PATH="/usr/local/opt/ruby/bin:$PATH"' >> ~/.zshrc

# Install Jekyll and other dependencies (may take a few minutes)
bundle install

# Run jekyll (s == serve)
bundle exec jekyll s

# The site should be running locally at http://localhost:4000

```

## Acknowledgments
This site is based of off the Jekyll theme Compass. See here for more info: https://excentris.github.io/compass/
