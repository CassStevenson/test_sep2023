---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.17.2 <!--0.13-->
    jupytext_version: 6.5.4 <!-- 1.16.4-->
kernelspec:
  display_name: Python 3
  language: python
  name: python3
editor_options: 
  markdown: 
  wrap: none
---
(i_sp_asymptote)=
# {{ title_i_sp_asymptote }}

:::::::::{div} full-width

:::::::{tab-set}

::::::{tab-item} Overview
To understand what we mean when we say, “species-accumulation asymptote”, we must first explain species accumulation curves. A **species accumulation curve** shows you the relationship between the number of species detected and sampling effort ({{ ref_intext_deng_et_al_2015 }})  (e.g., how you might expect to “accumulate” detections of new species as cameras are deployed for longer). Species accumulation curves are used "to assess and compare diversity across populations, or to evaluate the benefits of additional sampling" ({{ ref_intext_vandooren_2016 }}). The **species-accumulation *asymptote*** refers to the point on the curve where you’ve sampled long enough to observe *most* of the species present.

Consider the figure below. You can see that as the “number of records” (on the x-axis) increases, at first (where the line is the steepest), you detect new species quickly. This is because many species that are easy to detect and/or common, and thus you’re more likely to encounter them in less time. As time goes on (you collect more samples), the rate at which you detect *new* species starts to slow down (fewer and fewer new species detected over the same amount of time). This is because, in general, rare species, occurring much less often, may be missed if sampling is not long enough to detect it (or to be sure that they will not be detected). The curve starts to level off as after you’ve detected most (or all) of the easily detectable/common species and are slowly detecting those that are less detectable and/or rarer. As this line flattens out, eventually, barely any new species are detected (if any).

```{figure} ../03_images/03_image_files/loreau_2010_fig4_clipped.png
:width: 700px
:align: center
```

**Loreau (2010) - Fig 4** - “Species accumulation and rarefaction curves. Species accumulation curves show the number of species obtained by successively censusing either individual organisms (individual-based accumulation curves) or samples (sample-based accumulation curves).... Credit: Rob Colwell, after Gotelli and Colwell (2001)”

**<font size="4"><span style="color:#2F5496">How does this relate to study design?</font></span>**

This question is related to the state variable “Species Diversity & Richness”

Whether or not you choose to sample long enough to ensure to reach the species-accumulation asymptote will impact the number of cameras recommended; published species-accumulation curves for remote camera data seem to suggest that species level off between 20 and 100 locations ({{ ref_intext_ahumada_et_al_2011 }}; {{ ref_intext_li_et_al_2012 }}; {{ ref_intext_wearn_et_al_2016 }}). It will also impact the available modelling approaches since it not always necessary; some non-parametric methods are thought to estimate asymptotic richness fairly well “even when extrapolating to double or triple the size of the sample” ({{ ref_intext_colwell_et_al_2012 }}; {{ ref_intext_wearn_gloverkapfer_2017 }}). 

> **If you’re not sure, select the conservative answer of “Yes”**

::::::

::::::{tab-item} Advanced
```{figure} ../03_images/03_image_files/00_coming_soon.png
:width: 300px
:align: center
```
::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_gotelli_chao_2013 }}
```{figure} ../03_images/03_image_files/gotelli_chao_2013_fig4_clipped.png 
:width: 100%
:align: center
```
**Gotelli & Chao (2013) – Fig. 4** Standardized comparison of species richness for two individual-based rarefaction curves. 
:::{dropdown}
The data represent summary counts of carabid beetles that were pitfall-trapped from a set of young pine plantations (o20 years old; upper curve) and a set of old pine plantations (20–60 years old; lower curve). The solid lines are the rarefaction curves, calculated from eqn [2], and the shaded polygons are the 95% confidence intervals, calculated from the unconditional variance eqn [5]. The young plantation samples contained 243 individuals representing 31 species, and the old plantation samples contained 63 individuals representing nine species. The dashed and dotted vertical line illustrates a species richness comparison standardized to 63 individuals, which was the observed abundance in the smaller of the two data sets. Data from Niemel ̈a J, Haila Y, Halme E, et al. (1988) The distribution of carabid beetles in fragments of old coniferous taiga and adjacent managed forest. Annales Zoologici Fennici 25: 107–199.
:::
::::

::::{grid-item-card} {{ ref_intext_gotelli_colwell_2011 }}
```{figure} ../03_images/03_image_files/gotelli_and_colwell_2011_fig4_1_clipped.png
:height: 300px
:align: center
```

**Gotelli & Colwell (2011) - Fig. 4.1** Species accumulation and rarefaction curves.
:::{dropdown}
The jagged line is the species accumulation curve for one of many possible orderings of 121 soil seedbank samples, yielding a total of 952 individual tree seedlings, from an intensive census of a plot of Costa Rican rainforest (Butler & Chazdon 1998). The cumulative number of tree species (y-axis) is plotted as a function of the cumulative number of samples (upper x-axis), pooled in random order. The smooth, solid line is the sample-based rarefaction curve for the same data set, showing the mean number of species for all possible combinations of 1, 2, . . . , m∗, . . . , 121 actual samples from the dataset—this curve plots the statistical expectation of the (sample-based) species accumulation curve. The dashed line is the individual-based rarefaction curve for the same data set—the expected number of species for (m∗) (952/121) individuals, randomly chosen from all 952 individuals (lower x-axis). The black dot indicates the total richness for all samples (or all individuals) pooled. The sample-based rarefaction curve lies below the individual-based rarefaction curve because of spatial aggregation within species. This is a very typical pattern for empirical comparisons of sample-based and individual-based rarefaction curves.
:::

::::

::::{grid-item-card} {{ ref_intext_vandooren_2016 }}
```{figure} ../03_images/03_image_files/vandooren_2016_fig1_clipped.png 
:width: 100%
:align: center
```
**Van Dooren (2015) – Fig. 1** “Species accumulation curves. Species richness is the asymptote of a species accumulation curve, which expresses the dependence on sampling effort of the number of species sampled from an assemblage.
:::{dropdown}
In CA2013, sampling effort is given by the number of records from which the number of species is calculated. For illustrative purposes, an example with three arbitrary samples (for 10000, 5000 and 2000 records, labeled from one to three) is drawn. For sample one, a predicted species accumulation curve is added that gradually increases from one species sampled to the predicted species richness for that assemblage (full line). Such curves are constructed on the basis of interpolation and extrapolation. For samples two and three only segments of extrapolated curves are drawn (dotted lines). For sample two, a curve that crosses the species accumulation curve of sample one is sketched. For samples one and three species accumulation curves are more or less proportional. The way in which the species richness differences between samples are assessed in CA2013 is illustrated by indicating on the species accumulation curves at which numbers of records pairwise comparisons would be made between two sample pairs (1 vs. 2 and 1 vs. 3). The number of species of the sample with the smallest number of records is extrapolated to the number expected at three times the number of records. When the number of records of the other sample is still larger than that, the number of species of the second sample is interpolated (rarefied), otherwise it is extrapolated as well.
:::
::::

:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_loreau_2010 }}
```{figure} ../03_images/03_image_files/loreau_2010_fig4_clipped.png 
:width: 100%
:align: center
```
**Loreau (2010) – Fig. 4** - Species accumulation and rarefaction curves. Species accumulation curves show the number of species obtained by successively censusing either individual organisms (individual-based accumulation curves) or samples (sample-based accumulation curves). Smoothed species rarefaction curves represent the statistical expectation of the corresponding accumulation curves. Credit: Rob Colwell, after Gotelli and Colwell (2001)
::::

::::{grid-item-card} {{ ref_intext_molloy_2018 }}
```{figure} ../03_images/03_image_files/molloy_2018_fig9_clipped.png 
:width: 100%
:align: center
```
**Molloy (2018) – Fig. 9** Species accumulation curve for camera trap data collected in Dryandra Woodland. Sourced from Thomas & Cowan (2016) 
::::

::::{grid-item-card} {{ ref_intext_rovero_tobler_2010 }}
```{figure} ../03_images/03_image_files/rovero_tobler_2010_fig4.png
:width: 100%
:align: center
```
**Rovero & Tobler (2010) - Fig. 4.** Raw (dashed line) and rarefied (continuous line) species accumulation curves for camera-trap inventory data from the Peruvian Amazon.
::::
:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_rk_stats_2018 }}
<iframe 
    width="100%"
    height="300"
    src="https://www.youtube.com/embed/Jj7LYrU_6RA?si=odfIIBoC2w9h3_CU"
    loading="lazy
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

Species Accumulation Curves (11 minutes)
::::

::::{grid-item-card} {{ ref_intext_styring_2020b }} 
<iframe 
    width="100%"
    height="300"
    src="https://www.youtube.com/embed/OEWdPm3zg9I?si=2RG41LmTRvWfMiEr"
    loading="lazy"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

Generating a species accumulation plot in excel for BBS data
::::

::::{grid-item-card} {{ ref_intext_wildlifedegree_2022 }}
<iframe 
    width="100%"
    height="300"
    src="https://www.youtube.com/embed/h3MLWK9IJ4A?si=qOKB8jyALD3cwgAe"
    loading="lazy"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

Rarefied Species Accumulation Curves (the simple way) tutorial: How to create beautiful rarefied species accumulation curves with species richness, shannon wiener or the simpson index with abundance data, or species richness with incidence data using the iNext Online interface (which runs the iNext R package in the background)
::::
:::::

::::::

::::::{tab-item} Shiny apps/Widgets
:::::{card}
<iframe 
    width="100%"
    height="900"
    src="https://chao.shinyapps.io/iNEXTOnline"
    loading="lazy"
    frameborder="0" 
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

:::::

::::::

::::::{tab-item} Analytical tools & resources
| Type | Name | Note | URL |Reference |
|:----------------|:-------------------------------|:----------------------------------------------------------------|:----------------------|:----------------------------------------|
| R package / Tutorial | Species Accumulation Curves |      | <https://www.pisces-conservation.com/sdrhelp/index.html?specaccum.html> | {{ ref_bib_chao_et_al_2016 }} |
| R package / Tutorial | Species Accumulation Curves with vegan, BiodiversityR and ggplot2 |      | <https://rpubs.com/Roeland-KINDT/694021> | {{ ref_bib_roeland_2020 }} |
| R Shiny App | iNext Online |      | <https://chao.shinyapps.io/iNEXTOnline> | {{ ref_bib_chao_et_al_2016 }} |
| R package | Package ‘iNEXT’ - Interpolation and Extrapolation for Species Diversity |      | <https://cran.r-project.org/web/packages/iNEXT/iNEXT.pdf> | {{ ref_bib_chao_et_al_2016 }} |
| Video | iNext Online - Rarefied Species Accumulation Curves (the simple way) tutorial | Video to accompany the “iNext Online” R Shiny App | <https://www.youtube.com/watch?v=h3MLWK9IJ4A> | {{ ref_bib_wildlifedegree_2022 }} |
::::::

::::::{tab-item} References
{{ ref_bib_ahumada_et_al_2011 }}

{{ ref_bib_chao_et_al_2016 }}

{{ ref_bib_colwell_et_al_2012 }}

{{ ref_bib_deng_et_al_2015 }}

{{ ref_bib_gotelli_colwell_2001 }}

{{ ref_bib_gotelli_colwell_2011 }}

{{ ref_bib_li_et_al_2012 }}

{{ ref_bib_loreau_2010 }}

{{ ref_bib_molloy_2018 }}

{{ ref_bib_roeland_2020 }}

{{ ref_bib_rk_stats_2018 }}

{{ ref_bib_rovero_tobler_2010 }}

{{ ref_bib_si_et_al_2014 }}

{{ ref_bib_styring_2020b }}

{{ ref_bib_vandooren_2016 }}

{{ ref_bib_wearn_gloverkapfer_2017 }}

{{ ref_bib_wearn_et_al_2016 }}

{{ ref_bib_wildlifedegree_2022 }}
::::::

:::::::

:::::::::