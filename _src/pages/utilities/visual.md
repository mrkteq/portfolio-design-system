---
title: Visual
eleventyNavigation:
  key: Visual
  parent: Utilities
  order: 5
---

{% import 'macros/code.njk' as code %}

## Margin Auto

Use `.mrk-margin-auto` to center an element.

**Example**  
A centered image using margin auto.

<div class="doc-example">
  <figure>
    <img src="/assets/images/mark.jpg" class="mrk-avatar mrk-margin-auto mrk-stack-xs" alt="Mark">
    <figcaption class="mrk-text-body-sm mrk-text-center">
      Mark Tucker
    </figcaption>
  </figure>
</div>

{% call code.sample() %}
<figure>
  <img src="mark.jpg" class="mrk-avatar mrk-margin-auto mrk-stack-xs" alt="Mark">
  <figcaption class="mrk-text-body-sm mrk-text-center">
    Mark Tucker
  </figcaption>
</figure>
{% endcall %}
