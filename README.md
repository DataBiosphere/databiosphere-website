# databiosphere-website

[![Build Status](https://travis-ci.org/DataBiosphere/databiosphere-website.svg?branch=master)](https://travis-ci.org/DataBiosphere/databiosphere-website)

A place to collect content for a data biosphere website.  Right now this is just a template and has no content.

## Hugo-based Data Biosphere Website

This uses [Hugo](https://gohugo.io/) which lets us write content in Markdown and apply themes to get a pretty website.

### Organization

Things we want to touch on in the website:

* vision, mission... Apache for biomedical research
  * diagram: updated version of the arch diagram
  * who's a part of Data Biosphere
  * join us, learn more
* implementations
  * modules and data environments
  * diagram: examples in practice
  * datasets connected with the implementations
* Who benefits from the Data Biosphere?  
  * Funders - efficiency, repository of reusable vetted components
  * Data Creators & Stewards - off-the-shelf standards based interoperabile components
  * Tool Developers - distribution platform that supports open source licenses
  * Researchers (Consumers) - trusted components that support the community. Share my work with like-minded researchers
  * Public? Cloud Vendors? System Integrators? Others? be able to speak to the benefits for other groups too
* Getting involved, how we add new groups/projects/companies/etc.

### Next steps:
* get happy with the outline above
* Brian to make placeholders for the above, work on auto-deployment
* Danielle to help give feedback on the template and suggest changes to layout/images, graphics
* Sean and all of us helping to refine and get feedback on the site from PIs and others... fill in gaps we have right now

## Automatic Deployment

This repo is setup to automatically build on [TravisCI](https://travis-ci.org/DataBiosphere/databiosphere-website) and deploy to GitHub pages.  This means any changes you make to the files here will automatically deployed to https://databiosphere.github.io/databiosphere-website/

## Install

Setup on a mac:

    brew install hugo

## Start Server

    cd databiosphere
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

## Useful References

I found the following very helpful when setting this up:

* [How to create a website like freshswift.net using Hugo, Travis CI, and GitHub Pages](https://medium.com/zendesk-engineering/how-to-create-a-website-like-freshswift-net-using-hugo-travis-ci-and-github-pages-67be6f480298)
* [Hugo, Github, Travis: a step in continuous deployment!](https://insileco.github.io/2018/03/30/hugo-github-travis-a-step-in-continuous-deployment/)
* this site layout is based on the [Hugo Fresh theme](https://themes.gohugo.io/hugo-fresh/)
