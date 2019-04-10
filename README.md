# databiosphere-website

A place to collect content for a data biosphere website.  Right now this is just a template and has no content.

## Hugo-based Website

This uses Hugo

## Install

Setup on a mac:

    brew install hugo

## Start Server

    hugo server

And view the site on http://localhost:1313/

## Creating the Site

This is already done for you but this is how I did it:

```
brew install hugo
hugo new site databiosphere
cd databiosphere

# Clone the Fresh theme
git clone https://github.com/StefMa/hugo-fresh themes/hugo-fresh

# Remove the default config
rm config.toml

# Fetch the example config
curl -O https://raw.githubusercontent.com/StefMa/hugo-fresh/master/exampleSite/config.yaml

# Run the site locally
hugo server

# Open the site in your browser
open http://localhost:1313
```
