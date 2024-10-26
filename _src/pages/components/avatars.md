---
title: Avatars
eleventyNavigation:
  key: Avatars
  parent: Components
  order: 1
---

{% import 'macros/code.njk' as code %}

Use avatars to display a portrait of a person. Images with non-square aspect ratios will be cropped to the center. Be sure to include an `alt` attribute. Avatars come in two sizes.

<table class="doc-table">
  <tr>
    <th>Class</th>
    <th>Size</th>
  </tr>
  <tr>
    <td><code>.mrk-avatar</code></td>
    <td>90px</td>
  </tr>
  <tr>
    <td><code>.mrk-avatar-sm</code></td>
    <td>30px</td>
  </tr>
</table>

**Example**  
Default and small avatars.

<div class="doc-example doc-flow">
  <div class="doc-flex">
    <img class="mrk-avatar" src="/assets/images/mark.jpg" alt="Mark">
  </div>
  <div class="doc-flex">
    <img class="mrk-avatar-sm" src="/assets/images/mark.jpg" alt="Mark">
  </div>
</div>

{% call code.sample() %}
<img class="mrk-avatar" src="mark.jpg" alt="Mark">
<img class="mrk-avatar-sm" src="mark.jpg" alt="Mark">
{% endcall %}