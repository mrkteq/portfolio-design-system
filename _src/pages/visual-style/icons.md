---
title: Icons
eleventyNavigation:
  key: Icons
  parent: Visual Style
  order: 4
---

{% import 'macros/code.njk' as code %}

Icons are used in UI components to symbolize actions or provide additional visual context.

## Icon Set

<p>{{ iconlist.length }} icons</p>

<div class="mrk-grid" style="--grid-col-min: 150px; --gap: 12px">
{% for svg in iconlist %}
<figure class="mrk-flex">
  <svg aria-hidden="true" class="mrk-icon-24" data-icon="{{svg}}">
    <title>{{svg}}</title>
    <use xlink:href="#{{svg}}"></use>
  </svg>
  <figcaption><a href="/assets/icons/{{svg}}.svg" class="mrk-text-inherit" download>{{svg}}</a></figcaption>
</figure>
{% endfor %}
</div>

## Usage

Icons are compiled into an SVG sprite which can be included directly on each page rather than referencing individual external files. You can call one or more instances of an icon with the SVG `use` element. You can then apply classes to each instance to change its size, color and other properties.

**Example**  
An icon with default styling.

<div class="doc-example">
  {% icon "mrk-logo", "mrk-icon-96" %}
</div>

{% call code.sample() %}
<svg aria-hidden="true" class="mrk-icon-96">
  <title>mrk-logo</title>
  <use xlink:href="#mrk-logo"></use>
</svg>
{% endcall %}

## Size

The default size of an icon is 16x16 but you can append size values to `mrk-icon` to adjust the size.

<div class="mrk-grid" style="--grid-col-min: 150px; --gap: 12px">
  <figure class="mrk-flex">
    <svg aria-hidden="true" class="mrk-icon-12">
      <title>heart</title>
      <use xlink:href="#heart"></use>
    </svg>
    <figcaption><strong>.mrk-icon-12</strong></figcaption>
  </figure>
  <figure class="mrk-flex">
    <svg aria-hidden="true" class="mrk-icon">
      <title>heart</title>
      <use xlink:href="#heart"></use>
    </svg>
    <figcaption><strong>.mrk-icon</strong></figcaption>
  </figure>
  <figure class="mrk-flex">
    <svg aria-hidden="true" class="mrk-icon-24">
      <title>heart</title>
      <use xlink:href="#heart"></use>
    </svg>
    <figcaption><strong>.mrk-icon-24</strong></figcaption>
  </figure>
</div>

## Color

The icons' SVG paths are set to inherit the color of their parent element. This means you can apply [text color utilities](/utilities/color/) to an icon to change its color.

**Example**  
Using text color utilities to change an icon's color.

<div class="doc-example">
  {% icon "mrk-logo", "mrk-icon-96 mrk-text-interactive" %}
</div>

{% call code.sample() %}
<svg aria-hidden="true" class="mrk-icon-96 mrk-text-interactive">
  <title>mrk-logo</title>
  <use xlink:href="#mrk-logo"></use>
</svg>
{% endcall %}

## Icon Guidelines

In order to keep icons consistent:

* Use a 24x24 artboard
* Add 1-2px of space between the icon and the edge of the artboard
* Set fill color to black (#000000)
* Unify paths into a single compound path

Before adding icons to the system, you can use [SVGOMG](https://jakearchibald.github.io/svgomg/) to further optimize them.