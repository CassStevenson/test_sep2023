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
(i_mod_is)=
# {{ name_mod_is }}

**{{ term_mod_is }}**: {{ term_def_mod_is }}

::::::{dropdown} Assumptions, Pros, Cons
:::::{grid}

::::{grid-item-card} Assumptions
- {{ mod_is_assump_01 }}
- {{ mod_is_assump_02 }}
- {{ mod_is_assump_03 }}
- {{ mod_is_assump_04 }}
- {{ mod_is_assump_05 }}
::::
::::{grid-item-card} Pros
- {{ mod_is_pro_01 }}
- {{ mod_is_pro_02 }}
::::
::::{grid-item-card} Cons
- {{ mod_is_con_01 }}
- {{ mod_is_con_02 }}
- {{ mod_is_con_03 }}
::::
:::::
::::::

:::::::{tab-set}

::::::{tab-item} Overview
This section will be available soon! In the meantime, check out the information in the other tabs!

```{figure} ../03_images/03_image_files/00_coming_soon.png
:width: 300px
:align: center
```
::::::

::::::{tab-item} Advanced
:::{note}
**This content was adapted from**: The Density Handbook, "[Using Camera Traps to Estimate Medium and Large Mammal Density: Comparison of Methods and Recommendations for Wildlife Managers](https://www.researchgate.net/publication/368601884_Using_Camera_Traps_to_Estimate_Medium_and_Large_Mammal_Density_Comparison_of_Methods_and_Recommendations_for_Wildlife_Managers)" (Clarke et al., 2024)
:::

The instantaneous sampling model (IS) is an extension of the space-to-event model (STE; see above) that uses counts of animals in time-lapse images – instead of the area until an animal is first detected – to estimate density ({{ ref_intext_moeller_et_al_2018 }}). As with the STE, all cameras in a randomly-deployed array are programmed to take time-lapse images at predefined intervals (e.g., every hour) to get instantaneous “snapshot” samples of the study area. During image processing, the number of animals in each photograph is recorded. Thus, the IS is essentially a series of fixed-area point counts ({{ ref_intext_moeller_et_al_2018 }}): camera traps act as “standing observers” tabulating the number of individuals seen within a set area and time. 
The IS equation is as follows: 

```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_is1.png
:align: center
```

where *𝐽* is the total number of sampling occasions, *𝑀* is the total number of camera stations, and *𝑛<sub>𝑚𝑗</sub>* is the count of animals in the viewshed and *𝑎<sub>𝑚𝑗</sub>*  is the area of the viewshed at station *𝑚* on sampling occasion *𝑗* ({{ ref_intext_moeller_et_al_2018 }}).

## Simulations and Field Experiments

The IS is relatively untested opposite its sister models. Simulations have shown that the IS is unbiased to animal movement speed or population size, so is applicable to slow- and fast-moving animals and to low- and high-density populations ({{ ref_intext_moeller_et_al_2018 }}). When tested on a population of elk in Idaho, the IS produced a similar density estimate as an aerial survey, but which was less precise than both TTE- and STE-derived estimates ({{ ref_intext_moeller_et_al_2018 }}).
::::::

::::::{tab-item} Visual resources
:::::{grid} 3
:gutter: 1
:padding: 0
:margin: 0

::::{grid-item-card} {{ ref_intext_moeller_lukacs_2022 }}
```{figure} ../03_images/03_image_files/moeller_lukacs_2022_fig1.png
:class: img_grid
```
**Moeller & Lukacs (2022)** The spaceNtime workflow for count data. The user will go through five major steps for STE, TTE, and IS analyses. If the user has presence/absence (0 and 1) data instead of count data, the IS analysis is not appropriate, and the IS pathway should be removed from the flowchart.
::::

::::{grid-item-card} {{ ref_intext_clarke_et_al_2023 }}
```{figure} ../03_images/03_image_files/clarke_et_al_2023_eqn_is1.png 
:class: img_grid
```
  
::::

:::::

::::::

::::::{tab-item} Shiny apps/Widgets
Check back in the future!
::::::

::::::{tab-item} Analytical tools & resources
| Type | Name | Note | URL |Reference |
| resource15_type | resource15_name | resource15_note | resource15_url | {{ ref_bib_resource15_ref_id }} |
::::::

::::::{tab-item} References
{{ ref_bib_clarke_et_al_2023 }}

{{ ref_bib_moeller_et_al_2018 }}

{{ ref_bib_moeller_lukacs_2022 }}
::::::

:::::::