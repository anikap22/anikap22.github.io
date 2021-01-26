---
permalink: /projects/
title: "Porfolio"
classes: wide
layout: collection
collection: portfolio
entries_layout: grid
header:
    teaser: /assets/images/mtns_thin.jpg

excerpt: "Foo Bar design system including logo mark, website design, and branding applications."
header:
  image: /assets/images/mtns_thin.jpg
  teaser: /assets/images/mtns_thin.jpg

gallery_static:
  - url: /assets/images/tb_top10_time.png
    image_path: assets/images/tb_top10_time.png
    alt: "TB project"
  - url: /assets/images/no2.png
    image_path: assets/images/no2.png
    alt: "NO2 pollution"
  - url: /assets/images/DSC_0363.jpg
    image_path: assets/images/DSC_0363.jpg
    alt: "placeholder image 3"

gallery_interactive:
  - url: /assets/images/malaria_asia_static.png
    image_path: assets/images/malaria_asia_static.png
    alt: "placeholder image 1"
  - url: /assets/images/malaria_asia_static.png
    image_path: assets/images/malaria_asia_static.png
    alt: "placeholder image 2"
  - url: /assets/images/malaria_asia_static.png
    image_path: assets/images/malaria_asia_static.png
    alt: "placeholder image 3"

gallery_acrmap:
  - url: /assets/images/Arc_Nfix_precip2.png
    image_path: assets/images/Arc_Nfix_precip2.png
    alt: "nitrogen fixers and precipitation"
  - url: /assets/images/Arc_soilph_nfix.jpg
    image_path: assets/images/Arc_soilph_nfix.jpg
    alt: "nitrogen fixers and soil pH"

gallery_nfixest:
  - url: /assets/images/nfixest_fig1.png
    image_path: assets/images/nfixest_fig1.png
    alt: "estimate of n fixers across US"
  - url: /assets/images/nfixest_fig6.png
    image_path: assets/images/nfixest_fig6.png
    alt: "estimate of n inputs across US"

gallery_nfixneighbor:
  - url: /assets/images/nfixneighbor_fig1.png
    image_path: assets/images/nfixneighbor_fig1.png
    alt: "n fixer effect on neighbors"
  - url: /assets/images/nfixneibhor_fig3.png
    image_path: assets/images/nfixneighbor_fig3.png
    alt: "biotic interactions with n fixer effect on neighbor"

gallery_mlbgb:
  - url: /assets/images/soilthickenss.png
    image_path: assets/images/soilthickness.png
    alt: "soil thickness data for US"
  - url: /assets/images/rootsites.png
    image_path: assets/images/rootsites.png
    alt: "sites with bgb data"
---

## Visualizations
#### Static figures:
Static figures were produced both in R using packages such as `ggplot2` and `tmap` as well as in Python using `matplotlib` and `seaborn`.

{% include gallery id="gallery_static" caption="This is a sample gallery of static figures including (1) TB spending by country, (2) histogram of NO<sub>2</sub> emissions in US cities, and (3) ." %}

#### Interactive visualizations:
These interactive visualizations are examples of work that I can do for you and were produced in R using the `plotly` package.

Asian countries where mortality rates have declined over time:
<iframe src="/assets/images/malaria_asia.html" width="200%" height="550" id="igraph" scrolling="no" seamless="seamless" frameBorder="0"> </iframe>
African countries where mortality rates have declined over time:
<iframe src="/assets/images/malaria_africa.html" width="200%" height="550" id="igraph" scrolling="no" seamless="seamless" frameBorder="0"> </iframe>

#### ArcMap:
I have worked with geostatistics both in R and ArcMap. Here are a few example figures that I created using ArcMap.

{% include gallery id="gallery_acrmap" caption="This is a sample gallery to go along with this case study." %}

#### Shiny dashboards:
I can make interactive dashboards using R shiny. Here is an example:
<iframe src="https://cengiz-zopluoglu.shinyapps.io/names/" class="l-screen-inset shaded" height="1000px"></iframe>

## Projects
### Estimating nitrogen fixed across the U.S.
**Abstract:** <font size="3">Quantifying human impacts on the nitrogen (N) cycle and investigating natural ecosystem N cycling depend on the magnitude of inputs from natural biological nitrogen fixation (BNF). Here, we present two bottom-up approaches to quantify tree-based symbiotic BNF based on forest inventory data across the coterminous USA and SE Alaska. For all major N-fixing tree genera, we quantify BNF inputs using (1) ecosystem N accretion rates (kg N ha<sup>-1</sup> yr<sup>-1</sup>) scaled with spatial data on tree abundance and (2) percent of N derived from fixation (%Ndfa) scaled with tree N demand (from tree growth rates and stoichiometry). We estimate that trees fix 0.30-0.88 Tg N yr<sup>-1</sup> across the study area (1.4-3.4 kg N ha<sup>-1</sup> yr<sup>-1</sup>). Tree-based N fixation displays distinct spatial variation that is dominated by two genera, Robinia (64% of tree-associated BNF) and Alnus (24%). The third most important genus, Prosopis, accounted for 5%. Compared to published estimates of other N fluxes, tree-associated BNF accounted for 0.59 Tg N yr<sup>-1</sup>, similar to asymbiotic (0.37 Tg N yr<sup>-1</sup>) and understory symbiotic BNF (0.48 Tg N yr<sup>-1</sup>), while N deposition contributed 1.68 Tg N yr<sup>-1</sup> and rock weathering 0.37 Tg N yr<sup>-1</sup>. Overall, our results reveal previously uncharacterized spatial patterns in tree BNF that can inform large-scale N assessments and serve as a model for improving tree-based BNF estimates worldwide. This updated, lower BNF estimate indicates a greater ratio of anthropogenic to natural N inputs, suggesting an even greater human impact on the N cycle.</font> <br>

**Tools:** <font size="3"> Analyses were implemented in R using packages such as <code>data.table</code>, <code>RSQLite</code>, <code>dplyr</code>, and <code>ggplot2</code>.</font>

{% include gallery id="gallery_nfixest" caption="These are sample figures from the case study. The figure on the left shows the distriubtion of nitrogen fixing tress across the U.S. The figure on the right shows different nitrogen inputs including biotic and abiotic sources as well as the fraction of N inputs that come from nitrogen fixation." %}

### Effect of nitrogen fixing trees on forest carbon storage
**Abstract:** <font size="3"> Nitrogen (N)-fixing trees fulfill a unique and important biogeochemical role in forests through their ability to convert atmospheric N<sub>2</sub> gas to plant-available N. Due to their high N fixation rates, it is often assumed that N-fixing trees facilitate neighboring trees and enhance forest growth. This assumption is supported by some local studies but contradicted by others, leaving the overall effect of N-fixing trees on forest growth unresolved. Here we use the U.S. Forest Service’s Forest Inventory and Analysis database to evaluate the effects of N-fixing trees on plot-scale basal area change and individual-scale neighboring tree demography across the coterminous U.S. First we discuss the average trends. At the plot and individual scales, N-fixing trees do not affect the relative growth rates of neighboring trees, but they facilitate recruitment and inhibit survival rates, suggesting that they are drivers of tree turnover in the coterminous U.S. At the plot scale, N-fixing trees facilitate the basal area change of non-fixing neighbors. In addition to the average trends, there is wide variation in the effect of N-fixing trees on forest growth, ranging from strong facilitation to strong inhibition. This variation does not show a clear geographic pattern, though it does vary with certain local factors. N-fixing trees facilitate forest growth when they are likely to be less competitive: under high N deposition and high soil moisture or when neighboring trees occupy different niches (e.g. high foliar C:N trees and non-fixing trees). Overall, N-fixing trees have highly variable effects on forest growth and neighbor demographics across the coterminous U.S. This suggests that the effect of N-fixing trees on forest development and carbon storage depends on local factors, which may help reconcile the conflicting results found in previous localized studies on the effect of N-fixing trees on forest growth. </font> <br>

**Tools:** <font size="3"> Analyses were conducted in R using packages such as <code>dplyr</code>, <code>sp</code>, <code>raster</code>, <code>rgdal</code> and <code>ggplot2</code></font>

{% include gallery id="gallery_nfixneighbor" caption="These are key figures from the analysis. The figure on the left shows the effect of nitrogen fixing trees on growth, recruitment, and survival of neighboring trees. The figure on the right shows the abiotic interactions with the nitrogen fixing tree effect." %}

### Machine learning model to predict nitrogen fixing tree presence

### Machine learning model to predict belowground biomass

{% include gallery id="gallery_mlbgb" caption="These are sample figures from the machine learning model predicting belowground biomass from remote sensing metrics. The figure on the left shows soil thickness plotted using tmap and the figure on the right shows the sites across the globe where belowground biomass was measured." %}

