---
title: Color
eleventyNavigation:
  key: Color
  parent: Utilities
  order: 1
---

{% import 'macros/code.njk' as code %}

Color utilities can be used to apply specific colors to text, icons, and backgrounds.

## Text

Use text utilities to change the color of text and icons.

**Example**  
Text and icons in different colors.

<div class="doc-example mrk-flow">
  <div class="mrk-surface mrk-inset-square mrk-text-subdued">
    <p><strong>.mrk-text-subdued</strong><br>
    Use subdued text to reduce emphasis independent of font size/weight.</p>
    {% icon "heart", "mrk-icon-24" %}
  </div>
  <div class="mrk-surface-brand mrk-inset-square mrk-text-inverse">
    <p><strong>.mrk-text-inverse</strong><br>
    Use inverse text to provide adequate contrast on dark backgrounds.</p>
    {% icon "heart", "mrk-icon-24" %}
  </div>
  <div class="mrk-surface-brand mrk-inset-square mrk-text-subdued-inverse">
    <p><strong>.mrk-text-subdued-inverse</strong><br>
    Use subdued inverse text to reduce emphasis on dark backgrounds.</p>
    {% icon "heart", "mrk-icon-24" %}
  </div>
</div>

{% call code.sample() %}
<div class="mrk-surface mrk-text-subdued">
  <p><strong>.mrk-subdued</strong><br>
  Use subdued text to reduce emphasis independent of font size/weight.</p>
  <svg aria-hidden="true" class="mrk-icon-24">
    <title>heart</title>
    <use xlink:href="#heart"></use>
  </svg>
</div>
<div class="mrk-surface-brand mrk-text-inverse">
  <p><strong>.mrk-text-inverse</strong><br>
  Use inverse text to provide adequate contrast on dark backgrounds.</p>
  <svg aria-hidden="true" class="mrk-icon-24">
    <title>heart</title>
    <use xlink:href="#heart"></use>
  </svg>
</div>
<div class="mrk-surface-brand mrk-text-subdued-inverse">
  <p><strong>.mrk-text-subdued-inverse</strong><br>
  Use subdued inverse text to reduce emphasis on dark backgrounds.</p>
  <svg aria-hidden="true" class="mrk-icon-24">
    <title>heart</title>
    <use xlink:href="#heart"></use>
  </svg>
</div>
{% endcall %}

## Inherit

Use the inherit utility to make an element's content inherit the text color of its parent. Useful for overriding the default color of links.

**Example**  
A default link and a link with inherit applied.

<div class="doc-example mrk-flow">
  <p><a href="https://mrkteq.netlify.app">Mrkteq | Portfolio</a></p>
  <p><a href="https://mrkteq.netlify.app" class="mrk-text-inherit">Mrkteq | Portfolio</a></p>
</div>

{% call code.sample() %}
<p><a href="https://mrkteq.netlify.app">Mrkteq | Portfolio</a></p>
<p><a href="https://mrkteq.netlify.app" class="mrk-text-inherit">Mrkteq | Portfolio</a></p>
{% endcall %}

## Surface

Use surface utilities to change the background color of an element.

**Example**  
Containers with different background colors.

<div class="doc-example mrk-flow">
  <div class="doc-bordered mrk-surface mrk-inset-square">
    <strong>.mrk-surface</strong>
  </div>
  <div class="doc-bordered mrk-surface-brand mrk-inset-square mrk-text-inverse">
    <strong>.mrk-surface-brand</strong>
  </div>
</div>

{% call code.sample() %}
<div class="mrk-surface mrk-inset-square">
  <strong>.mrk-surface</strong>
</div>
<div class="mrk-surface-brand mrk-inset-square mrk-text-inverse">
  <strong>.mrk-surface-brand</strong>
</div>
{% endcall %}