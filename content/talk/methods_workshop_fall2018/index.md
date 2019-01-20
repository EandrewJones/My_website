+++
title = "How to Scrape the Web using R"
subtitle = "A workshop and associated R package"
date = 2018-12-21T00:00:00  # Schedule page publish date.
draft = false

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
time_start = 2018-10-01T14:00:00
time_end = 2018-10-01T15:10:00

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Evan Jones"]

# Abstract and optional shortened version.
abstract = "Web scraping is a powerful tool for mining large amounts of data. Though Python has traditionally been the preferred language for scraping, R offers an assortment of competitive packages for tasks ranging from simple scrapes to crawling the web. In this talk, I teach the essentials of web scraping via a custom-built R package, <i>how2scrape</i>, available from my github."
abstract_short = ""

# Name of event and optional event URL.
event = "UMD Government and Politics Methods Workshop Fall 2018"
event_url = ""

# Location of event.
location = "Dept. of Government and Politics, UMD"

# Is this a selected talk? (true/false)
selected = false

# Projects (optional).
#   Associate this talk with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["deep-learning"]` references 
#   `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects = [""]

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Slides (optional).
#   Associate this talk with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references 
#   `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides = ""

# Links (optional).
url_pdf = ""
url_slides = ""
url_video = ""
url_code = ""

# Does the content use math formatting?
math = true

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
[image]
  # Caption (optional)
  caption = ""

  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Right"
+++

The entire workshop is bundled into my R package, *how2scrape*. Below are the instructions for how to install it and follow along with the workshop. I plan to update the package in the future, extending coverage to include crawling with *RSelenium*. There's a possibility I'll create a similar tutorial for crawling with Python too. Any updates will be posted to my blog.

__Instructions for the workshop:__

We will be conducting the web scraping workshop in R. To be able to follow along and get the most out of the session, some preparation is in order.

First, download and install the CSS [selector gadget](https://selectorgadget.com/) plug-in if you do not already have it. This nifty tool is a tremendous aid when web scraping, especially for beginners who are not familiar with javascript, html, and xml/xpath. 

Second, I have bundled the entire workshop into an R package. Please download it from my github repository. To do so, run the following code in R:
```r
install.packages('devtools')
devtools::install_github('EandrewJones/how2scrape', build_vignettes = TRUE)
```
__Note:__ You must include `build_vignettes = TRUE`, otherwise the lab will not work. Also, the package only works in `R version >= 3.5.1`, so please make sure your version of R is updated. If you are still using an outdated version, think of this as a friendly nudge. 

The can take a fairly long time to download and compile. Don't worry, this is normal. The package scrapes ~10k bills from Congress as it compiles, so please be patient. If you run into any issues, please leave me a message via email or on github.
