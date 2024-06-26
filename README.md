## Install dependencies

sudo apt-get install ruby-full build-essential zlib1g-dev

Avoid installing RubyGems packages (called gems) as the root user. Instead, set up a gem installation directory for your user account. The following commands will add environment variables to your ~/.bashrc file to configure the gem installation path:

```
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
Finally, install Jekyll and Bundler:
```

`gem install jekyll bundler`

Create new site: `jekyll new myblog`

Build the site and make it available on a local server.

`bundle exec jekyll serve`

Browse to http://localhost:4000

## Enable GitHub pages from /docs on main

## Enable GitHub Actions
Jekyll By GitHub Actions

# Bootstrap

`npm install bootstrap@5.3.3`

Add base.url - required for github pages

    <link rel="stylesheet" href="{{ site.baseurl }}/assets/css/styles.css">

change paths in bootstrap file: placed in _sass:
// Required
@import "../node_modules/bootstrap/scss/variables";

Create assets/css/styles.scss
---
---
@import "bootstrap";