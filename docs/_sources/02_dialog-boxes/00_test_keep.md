---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.17.2 <!--0.13-->
    jupytext_version: 1.16.4  <!--6.5.2-->
kernelspec:
  display_name: Python 3
  language: python
  name: python3
editor_options: 
  markdown: 
  wrap: none
---
# 00_test_embed --------------------------------------------------------------------

this one
```{include} include/00_test_image.md
```

this one
```{include} include/00_test_image.md
```

***

{ref}`*Access Method`


```{embed} #myLabel
```

1
```{embed} #myLabel
```


2
```{literalinclude} #myLabel
```


3
```{include}} #myLabel
```


4
```{embed} include/00_test_image.md#myLabel
```

5
```{literalinclude} include/00_test_image.md#myLabel
```


6
```{include}} 00_test_image.md#myLabel
```

:::{figure} ../03_images/03_image_files/clarke_et_al_2023_fig7_clipped.png 
:class: img_grid

> **Clarke et al. (2023) - Fig. 7** Measuring *𝑟* and *𝜃* by field trial. The perimeter of the detection zone is determined by approaching the camera from different angles and at different speeds, and noting where the camera’s sensor (red flash) detects motion (red dots).
:::

# 00_tooltip --------------------------------------------------------------------
<button type="button" class="btn btn-secondary" data-bs-toggle="tooltip" data-bs-placement="top" title="Tooltip on top">
  Tooltip on top
</button>


{bdg-link-white}`explicit title <https://ab-rcsc.github.io/rc-decision-support-tool_concept-library>`


```{button-link} https://ab-rcsc.github.io/rc-decision-support-tool_concept-library
:color: primary
:shadow:
:align: center
:tooltip: I am a tooltip
Concept library
```

<span class='underline example'>underline</span>

<button type="button" class="btn btn-secondary btn-sm" data-bs-toggle="tooltip" data-bs-placement="top" title="Tooltip on top">
  Tooltip on top
</button>
<button type="button" class="btn btn-secondary btn-sm" data-bs-toggle="tooltip" data-bs-placement="right" title="Tooltip on right">
  Tooltip on right
</button>
<button type="button" class="btn btn-secondary btn-sm" data-bs-toggle="tooltip" data-bs-placement="bottom" title="Tooltip on bottom">
  Tooltip on bottom
</button>
<button type="button" class="btn btn-secondary btn-sm" data-bs-toggle="tooltip" data-bs-placement="left" title="Tooltip on left">
  Tooltip on left
</button>
<br>


<br>

[<button type="button" class="btn btn-secondary btn-sm" data-bs-toggle="tooltip" data-bs-placement="top" title="Tooltip on top">
<span style="color:#2F5496"><u>Access Method</u></span></button>](#access_method)

<br>
jjjjjj

Here is some text [<button type="button" class="btn btn-secondary btn-sm" btn-border-width= "1px" data-bs-toggle="tooltip" data-bs-placement="top" title="Tooltip on top"><span class='underline'>Access Method</span></button>](#access_method) and more text

<span class='underline'>Access Method</span>

<br>

Here is some text <button type="button" class="btn btn-link btn-sm" data-bs-toggle="tooltip" data-bs-placement="top" title="The method used to reach the camera location (e.g., on...).">[Access Method](#access_method)</button> and more text

<br>

Here is some text <button type="button" class="btn btn-link btn-sm" data-bs-toggle="tooltip" data-bs-placement="top" title="The method used to reach the camera location (e.g., on...).">[Access Method](#access_method)</button> and more text

<br>
<button type="button" class="btn btn-secondary btn-sm" btn-border-width= "0px" data-bs-toggle="tooltip" data-bs-placement="top" title="Tooltip on top"><span class='underline'>Access Method</span></button>



<button type="button" class="btn btn-secondary btn-sm input-btn-padding-y-sm input-btn-padding-x-sm input-btn-font-size-sm" btn-border-width= "1px" data-bs-toggle="tooltip" data-bs-placement="top" title="Tooltip on top"><span class='underline'>Access Method</span></button>


{bdg-link-white}`explicit title <https://ab-rcsc.github.io/rc-decision-support-tool_concept-library>`


Here is some text [<span class='underline'>Access Method</span>](#access_method) Here is some text 

<button type="button" class="btn btn-primary btn-sm" data-bs-toggle="tooltip" data-bs-placement="right" title="Tooltip on right">
  Species Inventory
</button>




{bdg-link-white}`explicit title <https://ab-rcsc.github.io/rc-decision-support-tool_concept-library>`

<button type="button" class="btn btn-secondary position-relative">
  Inbox
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-warning">
    i
    <span class="visually-hidden">info</span>
  </span>
</button>

<br><br>

<button type="button" class="btn btn-secondary position-relative">
  Species Inventory
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-warning">
    i
    <span class="visually-hidden">info</span>
  </span>
</button>


<div class="d-grid gap-2 col-6 mx-auto">
  <button class="btn btn-primary position-relative" type="button">Button</button>
      <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-warning">
      i
      <span class="visually-hidden">info</span>
    </span>
  <button class="btn btn-primary position-relative" type="button">Button</button>
</div>




# 00_test_cross_ref --------------------------------------------------------------------
<iframe 
    width="100%"
    height="900"
    src="https://www.rc-decision-support-tool.ca/voila/render/objective.ipynb?"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
</iframe>

{ref}`*Access Method`  <!-- https://myst-parser.readthedocs.io/en/latest/syntax/optional.html#block-attributes-->

{ref}`your text here </09_glossary.md#deployment_comments>`

{ref}`your text here </09_glossary2.md#deployment_comments>`


<!-- worked to 09_glossary_blocktest.md-->

{term}`*Access Method`<!-- worked-->

{term}`term test<*Access Method>`<!-- worked-->

{ref}`ref text here<access_method>`

[test](access_method)  goes to page but not ref


`/09_glossary2.md#access_method`


[]{mods_zero_inflation}

'{'#access_method'}'

{#age_class_adult}

{age_class}



(heading-target)=
### Heading


.
.
.
.
.
.



{#paragraph-target}=
This is a paragraph, with an `id` attribute.

.
.
.
.
.
.

This is a [span with an `id` attribute]{#span-target}
.
.
.
.
.
.
.
.

:::{note}
:name: directive-target

This is a directive with a `name` option
:::
.
.
.
.
.
.
.

[heading link](#heading-target), [paragraph link](#paragraph-target),
[span link](#span-target), [directive link](#directive-target)

<!-- https://myst-parser.readthedocs.io/en/latest/syntax/cross-referencing.html--> 
<!-- https://pydata-sphinx-theme.readthedocs.io/en/stable/examples/kitchen-sink/generic.html#inline-hyperlink-targets--> 
<!-- https://docs.readthedocs.io/en/stable/guides/cross-referencing-with-sphinx.html#finding-the-reference-name--> 

<!-- WITH myst_heading_anchors: 3--> 
<!-- SAME WITH NO myst_heading_anchors: 3--> 
<!-- this is with target immediatiely after the id)--> 

<!-- (access_method)=
**\*Access Method--> 


[test](access_method)  ## goes to page but not ref

[test](#access_method) ## goes NOWHERE



[test](/09_glossary2.md#access_method)  ## unsure

[test](./09_glossary2.md#access_method) ## WORKS



[test](../09_glossary.md#access_method) ## goes to page but not ref

<!-- (#age_class_adult)=
**Adult**--> 
[test](/09_glossary.md#age_class_adult) ## goes to page but not ref

[test](./09_glossary.md#age_class_adult)## goes NOWHERE

[test](../09_glossary.md#age_class_adult) ## goes to page but not ref

<!-- now try with space no difference-->

# goes NOWHERE
 
[test]{/09_glossary.md#deployment_comments} 

[test]{./09_glossary.md#deployment_comments}

[test]{../09_glossary.md#deployment_comments}


[test]{/09_glossary.md#deployment_crew}

[test]{./09_glossary.md#deployment_crew}

[test]{../09_glossary.md#deployment_crew}

<!-- now try with space no difference-->