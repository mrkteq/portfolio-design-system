---
title: Buttons
eleventyNavigation:
  key: Buttons
  parent: Components
  order: 2
---

{% import 'macros/code.njk' as code %}

## Primary Button

Use the primary button as the main call-to-action on a page.

**Example**  
A primary button.

<div class="doc-example">
  <button type="button" class="mrk-button-primary button">Button</button>
</div>

{% call code.sample() %}
<button type="button" class="mrk-button-primary button">Button</button>
{% endcall %}

## Secondary Button

Use the secondary button as a regular button.

**Example**  
A secondary button.

<div class="doc-example">
  <button type="button" class="mrk-button-secondary">Button</button>
</div>

{% call code.sample() %}
<button type="button" class="mrk-button-secondary">Button</button>
{% endcall %}