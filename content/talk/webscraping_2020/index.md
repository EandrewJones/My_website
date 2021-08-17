+++
title = "Data Collection via Web Scraping"
subtitle = "A workshop and associated R package"
date = 2021-08-17T16:25:00  # Schedule page publish date.
draft = false

# Talk start and end times.
#   End time can optionally be hidden by prefixing the line with `#`.
time_start = 2020-10-20T16:00:00
time_end = 2020-10-01T17:15:00

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Evan Jones"]

# Abstract and optional shortened version.
abstract = "In this talk, I teach the essentials of web scraping via a custom-built R package, <i>how2scrape</i>, available from my github. I introduces some of the basic packages and tools available in the R language for web scraping and interfacing with APIs. Particular attention is paid to understanding the structure of websites and how they operate so that participants feel comfortable extrapolating beyond the presented examples to their own use cases.

The entire workshop is bundled into my R package, *how2scrape*. Below are the instructions for how to install it and follow along with the workshop. I plan to update the package in the future, extending coverage to include crawling with *RSelenium*. There's a possibility I'll create a similar tutorial for crawling with Python too. Any updates will be posted to my blog.

__Instructions for the workshop:__

We will be conducting the web scraping workshop in R. To be able to follow along and get the most out of the session, some preparation is in order.

First, download and install the CSS [selector gadget](https://selectorgadget.com/) plug-in if you do not already have it. This nifty tool is a tremendous aid when web scraping, especially for beginners who are not familiar with javascript, html, and xml/xpath. 

Second, I have bundled the entire workshop into an R package. Please download it from my github repository. To do so, run the following code in R:
```r
install.packages('devtools')
devtools::install_github('EandrewJones/how2scrape', build_vignettes = TRUE)
```
__Note:__ You must include `build_vignettes = TRUE`, otherwise the lab will not work. If asked to update any packages, please select none. Also, the package only works in `R version >= 3.5.1`, so please make sure your version of R is updated. If you are still using an outdated version, think of this as a friendly nudge. 

The can take a fairly long time to download and compile. Don't worry, this is normal. The package scrapes ~10k bills from Congress as it compiles, so please be patient. If you run into any issues, please leave me a message via email or on github.
"
abstract_short = ""

# Name of event and optional event URL.
event = "UMD Government and Politics Methods Workshop Fall 2020"
event_url = "https://github.com/gsa-gvpt/gvpt-methods/blob/master/webscraping/README.md"

# Location of event.
location = "Dept. of Government and Politics, UMD"

# Is this a selected talk? (true/false)
selected = true

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
url_pdf = "https://github.com/gsa-gvpt/gvpt-methods/blob/master/webscraping/README.md"
url_slides = "https://github.com/gsa-gvpt/gvpt-methods/blob/master/webscraping/README.md"
url_video = "https://www.dropbox.com/s/zndoq6v53xe85o6/web-scraping-jones.mp4?dl=0"
url_code = "https://github.com/EandrewJones/how2scrape"

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
