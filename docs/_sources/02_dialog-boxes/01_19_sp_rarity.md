---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.17.2 <!--0.13-->
    jupytext_version: 1.16.4 <!-- 6.5.4-->
kernelspec:
  display_name: Python 3
  language: python
  name: python3
editor_options: 
  markdown: 
  wrap: none
---
(i_sp_rarity)=
# {{ title_i_sp_rarity }}

:::{hint}
**Species rarity**: the number of individuals present of the species in question, relative to the total number of individuals of all species (or how “represented” is the species when considering the total number of individuals of all species).
While technically “how rare” a species is will be change from place to place (e.g., will depend on geographic range, habitat specificity, local abundance, etc.; {{ref_intext_crisfield_et_al_2024}}), for the purposes of informing study design recommendations, the **species rarity categories are defined as follows**:

- **Common**:  probability of occupancy > ~0.75-0.8  (> 0.75 [{{ref_intext_kinnaird_obrien_2012}}; {{ref_intext_kays_et_al_2020}}]; > 0.8 [{{ref_intext_shannon_et_al_2014}}; {{ref_intext_wearn_gloverkapfer_2017}}])
- **Less common**: 0.25-0.75
- **Rare**: probability of occupancy < 0.25 {{ref_intext_kays_et_al_2020}}
- **Very-rare**: probability of occupancy < 0.001 ({{ref_intext_wearn_gloverkapfer_2017}}; {{ref_intext_rowcliffe_et_al_2008}}; {{ref_intext_obrien_2010}})
- **Unknown**: select this option if you’re not sure of the rarity of your Target Species (single or multiple species)
- **Multiple**: select this option if your study includes multiple Target Species that vary in rarity.

Refer to the tabs below for more information.
:::

:::{seealso}
{bdg-link-primary-line}`Species-accumulation curves<https://ab-rcsc.github.io/rc-decision-support-tool_concept-library/02_dialog-boxes/01_10_sp_asymptote.html>`
{bdg-link-primary-line}`Species rarity<https://ab-rcsc.github.io/rc-decision-support-tool_concept-library/02_dialog-boxes/01_19_sp_rarity.html>`
:::

:::::::{tab-set}

::::::{tab-item} Overview
Generally, species rarity can be thought of as the probability that the species occupies the site, for a given species (or study area, depending on the scale of interest) {{ref_intext_kays_et_al_2020}}. 

::: {note}
Species rarity can be generally thought of as a species characteristic, however, “not in the same sense that hair colour or wing venation… it’ an emergent trait of a species' population and its environment rather than a trait of an individual organism” {{ref_intext_kunin_1997}}
:::

**<font size="4"><span style="color:#2F5496">How does this relate to study design?</font></span>**

**Species' rarity can influence the ideal camera arrangement. ** For example, when monitoring rare or cryptic species that are unlikely to be detected with other designs, it may be appropriate to use a *Targeted design* where cameras are placed in areas that are known or suspected to have higher activity levels (e.g., game trails, mineral licks, etc.). 

**Species' rarity can influence the ideal number of cameras and [survey](#survey) length** ({{ ref_intext_chatterjee_et_al_2021 }}). Low [detection probability](#detection_probability) of rare or cryptic species can result in imprecise estimates if there are too few cameras or if cameras are not deployed for long enough (e.g., {{ref_intext_steenweg_et_al_2019 }})). Chatterjee et al. (2021) suggested that for [occupancy models](#mods_occupancy) ({{ref_intext_mackenzie_et_al_2002 }}) of common species, to survey a minimum of 50 sites for 15–20 days. For rare, elusive species, they recommended surveying 100 sites at a minimum for 20–30 days ({{ref_intext_chatterjee_et_al_2021 }}).

**Species' rarity can influence the appropriate modelling approach.** For measures of species richness or diversity, it is presumed that a camera is active long enough to detect rare species that may occur at a specific location ({{ ref_intext_wearn_gloverkapfer_2017 }}). If this is not the case, the results will indicate that the species was not present when it was (i.e., a “false negative”).
::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_leroy_2024 }}
:::{figure} ../03_images/03_image_files/leroy_2024_Rarity_cutoff-point.png
:class: img_grid
:::
**Leroy (2024)** The rarity cut-off point is here defined as the threshold of occurrence below which species are considered rare.
::::

::::{grid-item-card} {{ ref_intext_leroy_2024 }}
:::{figure} ../03_images/03_image_files/leroy_2024_Weight_assignation-curve.png 
:class: img_grid
:::
**Leroy (2024)** Weight assignation curve adjusted to an arbitrary rarity cut-off.
::::

:::::

:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_mecks100_2018 }}
<div>
  <div style="position:relative;padding-top:56.25%;">
    <iframe src="https://www.youtube.com/embed/4gcmAUpo9TU?si=_S-JYDDskR8QbHs5" loading="lazy" frameborder="0" allowfullscreen
      style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe>
  </div>
</div>

Species accumulation and rarefaction curves
::::

::::{grid-item-card} {{ ref_intext_riffomonas_project_2022b }} 
<div>
  <div style="position:relative;padding-top:56.25%;">
    <iframe src="https://www.youtube.com/embed/ywHVb0Q-qsM?si=_xJ5jbFc6MDEQlAh " loading="lazy" frameborder="0" allowfullscreen
      style="position:absolute;top:0;left:0;width:100%;height:100%;"></iframe>
  </div>
</div>

Generating a rarefaction curve from collector's curves in R within the tidyverse (CC198)
::::

:::::

::::::

::::::{tab-item} Shiny apps/Widgets
Check back in the future!
::::::

::::::{tab-item} Analytical tools & Resources
| Type | Name | Note | URL |Reference |
|:----------------|:-------------------------------|:----------------------------------------------------------------|:----------------------|:----------------------------------------| 
| R package | Package ‘Rarity’: Calculation of Rarity Indices for Species and Assemblages of Species | Allows calculation of rarity weights for species and indices of rarity for assemblages of species according to different methods (Leroy et al. 2012, Insect. Conserv. Divers. 5:159-168 <doi:10.1111/j.1752-4598.2011.00148.x>; Leroy et al. 2013, Divers. Distrib. 19:794-803 <doi:10.1111/ddi.12040>). | <https://cran.r-project.org/web/packages/Rarity/> | {{ ref_bib_leroy_2023 }} |
| Online resource | Rarity Indices | Brief, understandable explanation of rarity indices | <https://borisleroy.com/en/research/rarity-indices/> | {{ ref_bib_leroy_2024 }} |
::::::

::::::{tab-item} References
{{ ref_bib_chatterjee_et_al_2021 }}

{{ref_bib_crisfield_et_al_2024}}

{{ ref_bib_flather_sieg_2007 }}

{{ ref_bib_kays_et_al_2020 }}

{{ ref_bib_kinnaird_obrien_2012 }}

{{ ref_bib_kunin_1997 }}

{{ ref_bib_leroy_2023 }}

{{ ref_bib_leroy_2024 }}

{{ref_bib_mackenzie_et_al_2002 }}

{{ref_bib_obrien_2010}}

{{ ref_bib_riffomonas_project_2022b }}

{{ ref_bib_rowcliffe_et_al_2008 }}

{{ ref_bib_shannon_et_al_2014 }}

{{ ref_bib_southwell_et_al_2019 }}

{{ref_bib_steenweg_et_al_2019 }}

{{ ref_bib_mecks100_2018 }}

{{ ref_bib_wearn_gloverkapfer_2017 }}	
::::::

:::::::