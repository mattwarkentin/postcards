# postcards

Create simple, beautiful personal websites and landing pages using only
R Markdown.

## Installation

``` r
remotes::install_github("seankross/postcards")
```

## Getting Started

Postcards includes four templates:
[Jolla](https://seankross.com/postcards-templates/jolla/),
[Jolla Blue](https://seankross.com/postcards-templates/jolla-blue/),
[Trestles](https://seankross.com/postcards-templates/trestles/),
and [Onofre](https://seankross.com/postcards-templates/onofre/).
Each site is optimized for being displayed on desktop and mobile.
The goal of the package is to make it easy for anyone to create a single page
personal website with one R Markdown document. I hope this package can quickly
demonstrate the power and possibilities of the R and R Markdown ecosystem to 
newcomers.

To get started customizing one of these templates you should use
RStudio. Once you open RStudio: select **File**, **New File**, **R Markdown**, 
then select **From Template** to choose which template you want to start with.
Select **OK** after you choose a name for the folder that will contain your 
site. This folder will contain two files: an R Markdown document with your
site's content, and a sample photo that you should replace.

If you are not using RStudio, you can create the corresponding template files
using the following commands:

``` r
rmarkdown::draft("index.Rmd", "Jolla", package = "postcards")
rmarkdown::draft("index.Rmd", "Jolla-Blue", package = "postcards")
rmarkdown::draft("index.Rmd", "Trestles", package = "postcards")
rmarkdown::draft("index.Rmd", "Onofre", package = "postcards")
```

To compile the self contained HTML file for your site, you can use the **Knit**
button in RStudio or you can use `rmarkdown::render("index.Rmd")`. 
The HTML file can then be easily deployed to 
[GitHub Pages](https://pages.github.com/) or
[Netlify Drop](https://app.netlify.com/drop).

## The Templates

### Jolla

<p align="center"><img src="man/figures/jolla-preview.png" width="800px"></p>

```
---
title: "Tobi Burns"
image: "tobi.jpg"
socials:
  - LinkedIn: 
      link: "https://linkedin.com/"
  - Twitter: 
      link: "https://twitter.com/"
  - GitHub: 
      link: "https://github.com/"
  - Email: 
      link: "mailto:email@email.com"
output:
  postcards::jolla
---
 
I am a classically trained data scientist living in the San Fransisco Bay Area. 
Currently I work on the Oculus team at Facebook. I love talking about baseball, 
true crime podcasts, and causal inference.
```

### Jolla Blue

<p align="center"><img src="man/figures/jolla-blue-preview.png" width="800px"></p>

```
---
title: "Xiang Guo"
image: "xiang.jpg"
socials:
  - LinkedIn: 
      link: "https://linkedin.com/"
  - Twitter: 
      link: "https://twitter.com/"
  - GitHub: 
      link: "https://github.com/"
  - Email: 
      link: "mailto:email@email.com"
output:
  postcards::jolla_blue
---
 
Raised in New Jersey by two lawyers, I am now an aspiring data artist and 
competitive rock climber. I moved to Seattle to fly floatplanes, but I got 
caught up in the startup world. Send me a WhatsApp message if you have good 
turnip prices.
```

### Trestles

<p align="center"><img src="man/figures/trestles-preview.png" width="800px"></p>

```
---
title: "Frank Hermosillo"
image: "frank.jpg"
socials:
  - LinkedIn: 
      link: "https://linkedin.com/"
  - Twitter: 
      link: "https://twitter.com/"
  - GitHub: 
      link: "https://github.com/"
  - Email: 
      link: "mailto:email@email.com"
output:
  postcards::trestles
---
 
## Bio

Frank Hermosillo studies neural networks and their applications at Google 
rain. His research focuses on differentiable network pruning approximation and 
decentralized gradient inversion mechanics. He frequently collaborates with 
researchers who study machine learning, computer vision, and cognitive science.
His work has been featured in WIRED, The Atlantic, Newsweek, and The New York 
Times Magazine.

## Education

**Massachusetts Institute of Technology** | Cambridge, MA

Ph.D. in Computer Science | September 2009 - May 2014

**The University of California, Berkeley** | Berkeley, CA

B.S. in Computer Science | September 2005 - May 2009

## Experience

**Google Brain** | Principle Investigator | January 2018 - Present

**Netflix** | Research Scientist | June 2014 - December 2017
```

### Onofre

<p align="center"><img src="man/figures/onofre-preview.png" width="800px"></p>

```
---
title: "Willkommen!"
image: "herzl.jpg"
color1: "#5A59A3"
color2: "#C66060"
angle: 130
socials:
  - YouTube: 
      link: "https://youtube.com/"
  - Vimeo: 
      link: "https://vimeo.com/"
  - Twitter: 
      link: "https://twitter.com/"
  - Email: 
      link: "mailto:email@email.com"
output:
  postcards::onofre
---
 
György Herzl is a filmmaker and computational storyteller based in Leipzig,
Germany. Their work has been featured at the Festival do Rio, Internationale
Filmfestspiele Berlin, Kunsthalle Basel, and the New Museum of Contemporary Art
in New York City. "ГУМ" is their latest project which examines the rise of
consumerism in post-Soviet republics.
```

## Code of Conduct

Please note that the postcards project is released with a [Contributor Code of Conduct](https://contributor-covenant.org/version/2/0/CODE_OF_CONDUCT.html). By contributing to this project, you agree to abide by its terms.
