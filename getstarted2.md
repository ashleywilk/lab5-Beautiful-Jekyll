# Welcome to Beautiful Jekyll!
# This config file is meant for settings that affect your entire website. When you first
# set up your website you should go through all these settings and edit them, but after
# the initial set up you won't need to come back to this file often.
# --- Required options --- #
# Name of website
title: Lab 5, Beautiful Jekyll
# Your name to show in the footer
author: Ashley Wilkerson

<div class="gs-section-01" markdown="1">

### 1. Fork the Beautiful Jekyll repository 

Fork the [repository](https://github.com/daattali/beautiful-jekyll) 
by clicking the Fork button on the top right corner in GitHub.

</div>

<div class="gs-section-02" markdown="1">
### 2. Build your website in 3 steps
...
</div>


# --- List of links in the navigation bar --- #
navbar-links:
  About Me: Hello, I am currently a student at Arizona State University studying program evaluation and data analysis. 
  Resources:
    - Beautiful Jekyll: 
    - Learn markdown: 
    - Getting Started: "getstarted"  
    - Table Demo: "table-demo" 
  Author's home: "arosenk2@asu.edu"
# --- Logo --- #
# Image to show in the navigation bar - works best with a square image
# Remove this parameter if you don't want an image in the navbar

# --- Footer social media links --- #
# Select the social network links that you want to show in the footer.
# Uncomment the links you want to show and add your information to each one.
social-network-links:
  email: "arosenk2@asu.edu"
  github: "ashleywilk"
linkedin:" ashleywilkerson"

rss-description: This website is a virtual proof that I'm awesome
# --- General options --- #
# Select which social network share links to show in posts
share-links-active:
  twitter: true
  facebook: true
  linkedin: true
  vk: false
# How to display the link to your website in the footer
# Remove this if you don't want a link in the footer
url-pretty: "MyWebsite.com"
# Excerpt word length - Truncate the excerpt of each post on the feed page to the specified number of words
excerpt_length: 50
# Whether or not to show an excerpt for every blog post in the feed page
feed_show_excerpt: true
# Whether or not to show a list of tags below each post preview in the feed page
feed_show_tags: true
# Add a search button to the navbar
post_search: true
# The keywords to associate with your website, for SEO purposes
#keywords: "my,list,of,keywords"
# --- Colours / background image --- #
# Personalize the colours in your website. Colour values can be any valid CSS colour
navbar-col: "#D8D2CB"
navbar-text-col: "#5A5A60"
navbar-border-col: "#F5F3F1"
page-col: "#6A8FA5"
text-col: "#5A5A60"
link-col: "#5A5A60"
hover-col: "#D8D2CB"
footer-col: "#D8D2CB"
footer-text-col: "#777777"
footer-link-col: "#404040"
# Alternatively, the navbar, footer, and page background can be set to an image
# instead of colour
#navbar-img: "/assets/img/bgimage.png"
#footer-img: "/assets/img/bgimage.png"
#page-img: "/assets/img/bgimage.png"
# Suggest a colour for mobile browsers to use as the browser's theme. This is only supported by a few mobile browsers.
#mobile-theme-col: "#0085A1"
# For any extra visual customization, you can include additional CSS files in every page on your site. List any custom CSS files here
#site-css:
#  - "/assets/css/custom-styles.css"
# If you have common JavaScript files that should be included in every page, list them here
#site-js:
#  - "/assets/js/custom-script.js"
# --- Web Analytics Section --- #
# Fill in your Google Analytics gtag.js ID to track your website using gtag
#gtag: ""
# Fill in your Google Analytics ID to track your website using Google Analytics
#google_analytics: ""
# Fill in your Cloudflare Analytics beacon token to track your website using Cloudflare Analytics
#cloudflare_analytics: ""
# Google Tag Manager ID
#gtm: ""
# Matomo (aka Piwik) Web statistics
# Uncomment the following section to enable Matomo. The opt-out parameter controls
# whether or not you want to allow users to opt out of tracking.
#matomo:
#  site_id: "9"
#  uri: "demo.wiki.pro"
#  opt-out: true
# --- Comments --- #
# To use Disqus comments, sign up to https://disqus.com and fill in your Disqus shortname (NOT the userid)
#disqus: ""
# To use Facebook Comments, create a Facebook app and fill in the Facebook App ID
#fb_comment_id: ""
# To use Utterances comments: (0) uncomment the following section, (1) fill in
# "repository" (make sure the repository is public), (2) Enable Issues in your repository,
# (3) Install the Utterances app in your repository https://github.com/apps/utterances
# See more details about the parameters below at https://utteranc.es/
#utterances:
#  repository: # GitHub username/repository eg. "daattali/beautiful-jekyll"
#  issue-term: title   # Mapping between blog posts and GitHub issues
#  theme: github-light # Utterances theme
#  label: blog-comments # Label that will be assigned to GitHub Issues created by Utterances
# To use Staticman comments, uncomment the following section. You may leave the reCaptcha
# section commented if you aren't using reCaptcha for spam protection. 
# Using Staticman requires advanced knowledge, please consult 
# https://github.com/eduardoboucas/staticman/ and https://staticman.net/ for further 
# instructions. For any support with staticman please direct questions to staticman and 
# not to BeautifulJekyll.
#staticman:
#  repository : # GitHub username/repository eg. "daattali/beautiful-jekyll"
#  branch     : master # If you're not using `master` branch, then you also need to update the `branch` parameter in `staticman.yml`
#  endpoint   : # URL of your deployment, with a trailing slash eg. "https://<your-api>/v3/entry/github/"
#  reCaptcha:   # (optional, set these parameters in `staticman.yml` as well) 
#    siteKey  : # You need to apply for a site key on Google
#    secret   : # Encrypt your password by going to https://<your-own-api>/v3/encrypt/<your-site-secret>
# --- Misc --- #
# Ruby Date Format to show dates of posts
date_format: "%B %-d, %Y"
# Facebook App ID
#fb_app_id: ""

<style>

.gs-section-01 h3 { 
     color: red }

.gs-section-01 p {
     font-size: 30px;
}

</style>


# --- You don't need to touch anything below here (but you can if you want) --- #
# Output options (more information on Jekyll's site)
timezone: "America/Toronto"
markdown: kramdown
highlighter: rouge
permalink: /:year-:month-:day-:title/
paginate: 5
kramdown:
  input: GFM
# Default YAML values (more information on Jekyll's site)
defaults:
  -
    scope:
      path: ""
      type: "posts"
    values:
      layout: "post"
      comments: true  # add comments to all blog posts
      social-share: true # add social media sharing buttons to all blog posts
  -
    scope:
      path: "" # any file that's not a post will be a "page" layout by default
    values:
      layout: "page"
# Exclude these files from production site
exclude:
  - CHANGELOG.md
  - CNAME
  - Gemfile
  - Gemfile.lock
  - LICENSE
  - README.md
  - screenshot.png
  - docs/
plugins:
  - jekyll-paginate
  - jekyll-sitemap
# Beautiful Jekyll / Dean Attali
# 2fc73a3a967e97599c9763d05e564189
