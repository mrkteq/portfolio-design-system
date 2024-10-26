---
title: Nav Bar
eleventyNavigation:
  key: Nav Bar
  parent: Components
  order: 4
---

{% import 'macros/code.njk' as code %}

The nav bar is a flex container with a semi-transparent background for placing on top of a background image. The small version uses a lighter background color, has less padding, and is an inline flex container rather than a block flex container.

You can override the default justification of the contents of the nav bar using the `--flex-justify` custom property.

<table class="doc-table">
  <tr>
    <th>Custom Property</th>
    <th>Default Value</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><code>--flex-justify</code></td>
    <td>flex-start</td>
    <td>Horizontal alignment of flex items (justify-content)</td>
  </tr>
</table>

**Example**  
A small nav bar and a default nav bar.

<div class="doc-example mrk-flow">
  <a href="" class="mrk-text-eyebrow-sm mrk-nav-bar-sm">
    <span>Manage your profile</span>
    <img class="mrk-avatar-sm" src="/assets/images/mark.jpg" alt="Mark">
  </a>
  <ul role="list" class="mrk-text-eyebrow-lg mrk-nav-bar">
    <li><a href="">Home</a></li>
    <li><a href="">About</a></li>
    <li><a href="">Projects</a></li>
    <li><a href="">Contacts</a></li>
    <li><a href="">More</a></li>
  </ul>
</div>

{% call code.sample() %}
<a href="" class="mrk-text-eyebrow-sm mrk-nav-bar-sm">
  <span>Manage your profile</span>
  <img class="mrk-avatar-sm" src="mark.jpg" alt="Mark">
</a>
<ul role="list" class="mrk-text-eyebrow-lg mrk-nav-bar">
  <li><a href="">Home</a></li>
  <li><a href="">About</a></li>
  <li><a href="">Projects</a></li>
  <li><a href="">Contacts</a></li>
  <li><a href="">More</a></li>
</ul>
{% endcall %}