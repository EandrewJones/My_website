+++
# Project title.
title = "Beyond the Assembly"
subtitle = "Estimating Multidimensional Foreign Policy Preferences from Multi-Modal Data"

# Date this page was created.
date = 2021-08-17T14:49:00

# Project summary to display on homepage.
summary = "Conventional approaches to estimating latent preferences are constrained not only by the dearth of data from which preferences can be learned, usually roll-call votes, but also by the assumptions and limitations built into the statistical models they use to estimate these preferences. I develop a flexible, non-parametric model that allows researchers to combine multi-modal data, such as speeches and votes, and extract ideal points along as many dimensions as are stably present."

# Tags: can be used for filtering projects.
# Example: `tags = ["machine-learning", "deep-learning"]`
tags = ["multidimensional-scaling", "Bayesian-non-parametrics", "international-organizations"]

# Optional external URL for project (replaces project detail page).
external_link = ""

# Slides (optional).
#   Associate this project with Markdown slides.
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

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
#url_custom = [{icon_pack = "fab", icon="twitter", name="Follow", url = "https://twitter.com/georgecushen"}]

# Featured image
# To use, add an image named `featured.jpg/png` to your project's folder. 
[image]
  # Caption (optional)
  caption = "Photo by rawpixel on Unsplash"
  
  # Focal point (optional)
  # Options: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight
  focal_point = "Smart"
+++

*Working Paper*

{{% staticref "files/beyond-the-assembly-paper.pdf" "newtab" %}}PDF{{% /staticref %}} | {{% staticref "files/BeyondTheAssembly_Presentation_Jones.pdf" "newtab" %}}Slides (old version){{% /staticref %}}

## Abstract

Conventional approaches to estimating latent preferences face numerous constraints. They are limited not only by the dearth of data from which preferences
can be learned, usually roll-call votes, but also by the assumptions and limitations built into the statistical models they use to estimate these preferences. Commonly employed models such as DW-Nominate from the legislative studies literature or Bailey, Strezhnev, and Voeten’s (2017) dynamic IRT from IR are no exception. Both are limited to roll-call votes and require a priori assumptions about the number of latent dimensions that must be validated a posteriori. 

I develop a flexible, non-parametric model that allows researchers to combine multi-modal data, such as speeches and votes, and extract ideal points along as many dimensions as are stably present. I validate the model by examining it’s performance on the UNGA voting dating, using Bailey and company’s ideal points as a baseline, and find evidence for upwards of three dimension. I also apply the model to combined UNGA votes and debates as well as UNGA votes and Universal Period Review statements, illustrating the model’s utility for estimating topic-specific preferences that are still
anchored to well-established latent constructs.


## Results

{{< figure src"dims-plot.png" title="<strong>Dimensionality of the $\mathbf{25^{th}}$--$\mathbf{72^{nd}}$ UN General Assembly.</strong> Points indicate the median posterior number of dimensions mmBPFA found after burn-in. Bars represent 95\% HPD intervals. The median number of dimensions across sessions is 3, indicated by the blue dotted-line." >}}

{{< figure src="sess70-dim-plot.png" title="<strong>Ideal Point-Dimension Scatter Plots for $\mathbf{70^{th}}$ Session of UNGA (2015--2016).</strong> (top) Dimension 1 (x-axis) versus Dimension 2 (y-axis). (bottom) Dimension 1 (x-axis) versus Dimension 3 (y-axis)." >}}

{{< figure src="issue-frames-plot.png" title="<strong>UNGA $\mathbf{69^{th}}$ Session Ideal Points by Dimension.</strong> Each panel displays the ten countries occupying each pole of the given dimension. Ideal points are estimated based on the median posterior draw, and black bars represent 95\% credible intervals." >}}
