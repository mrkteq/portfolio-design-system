---
title: Type
eleventyNavigation:
  key: Type
  parent: Components
  order: 5
---

{% import 'macros/code.njk' as code %}

## Dynamic Type

<div class="doc-example doc-flow">
  <div>
    <p class="mrk-display-2">I am <span class="mrk-text-color word"></span></p>
    <p class="mrk-text-body-sm"><strong>.mrk-display-2 .mrk-text-color .word</strong></p>
  </div>
</div>

{% call code.sample() %}
<p class="mrk-display-2">I am <span class="mrk-text-color word"></span></p>
{% endcall %}

## Display Type

<div class="doc-example doc-flow">
  <div>
    <p class="mrk-display-1">Hi, my name</p>
    <p class="mrk-text-body-sm"><strong>.mrk-display-1</strong></p>
  </div>

  <div>
    <p class="mrk-display-2">Hi, my name</p>
    <p class="mrk-text-body-sm"><strong>.mrk-display-2</strong></p>
  </div>

  <div>
    <p class="mrk-display-3">Hi, my name</p>
    <p class="mrk-text-body-sm"><strong>.mrk-display-3</strong></p>
  </div>

  <div>
    <p class="mrk-display-4">Hi, my name</p>
    <p class="mrk-text-body-sm"><strong>.mrk-display-4</strong></p>
  </div>
</div>

{% call code.sample() %}
<p class="mrk-display-1">Hi, my name</p>
<p class="mrk-display-2">View my work</p>
<p class="mrk-display-3">View my resume</p>
<p class="mrk-display-4">Contact me</p>
{% endcall %}

## Headings

<div class="doc-example doc-flow">
  <div>
    <p class="mrk-heading-1">Hi, my name</p>
    <p class="mrk-text-body-sm"><strong>.mrk-heading-1</strong></p>
  </div>

  <div>
    <p class="mrk-heading-2">Hi, my name</p>
    <p class="mrk-text-body-sm"><strong>.mrk-heading-2</strong></p>
  </div>

  <div>
    <p class="mrk-heading-3">Hi, my name</p>
    <p class="mrk-text-body-sm"><strong>.mrk-heading-3</strong></p>
  </div>

  <div>
    <p class="mrk-heading-4">Hi, my name</p>
    <p class="mrk-text-body-sm"><strong>.mrk-heading-4</strong></p>
  </div>
</div>

{% call code.sample() %}
<p class="mrk-heading-1">Hi, my name</p>
<p class="mrk-heading-2">View my work</p>
<p class="mrk-heading-3">View my resume</p>
<p class="mrk-heading-4">Contact me</p>
{% endcall %}

## Body Text

<div class="doc-example doc-flow">
  <div>
    <p class="mrk-text-body-md">Digital Media Specialist with a focus on Design and Development, eager to tackle challenging projects and deliver top-notch results. I prioritise continuous learning and keeping up with the latest technologies and I am confident in my ability to thrive in a collaborative team environment and make valuable contributions. </p>
    <p class="mrk-text-body-sm"><strong>.mrk-text-body-md</strong></p>
  </div>

  <div>
    <p class="mrk-text-body-sm">With a proven track record of dedication and expertise, I'm looking for a new and exciting opportunities and seeking to joining with a dynamic team.</p>
    <p class="mrk-text-body-sm"><strong>.mrk-text-body-sm</strong></p>
  </div>
</div>

{% call code.sample() %}
<p class="mrk-text-body-md">
Profile Image

I'm a Digital Media Specialist with a focus on Design and Development, eager to tackle challenging projects and deliver top-notch results. I prioritise continuous learning and keeping up with the latest technologies and I am confident in my ability to thrive in a collaborative team environment and make valuable contributions. </p>
<p class="mrk-text-body-sm">My whole life philosophy sounds kinda silly when I say it out loud.</p>
{% endcall %}

## Eyebrows

<div class="doc-example doc-flow">
  <div>
    <p class="mrk-text-eyebrow-lg">Socials</p>
    <p class="mrk-text-body-sm"><strong>.mrk-text-eyebrow-lg</strong></p>
  </div>

  <div>
    <p class="mrk-text-eyebrow-sm">External links</p>
    <p class="mrk-text-body-sm"><strong>.mrk-text-eyebrow-sm</strong></p>
  </div>
</div>

{% call code.sample() %}
<p class="mrk-text-eyebrow-lg">Socials</p>
<p class="mrk-text-eyebrow-sm">External links</p>
{% endcall %}

## Emphasis

<div>
  <p class="mrk-text-subdued">Use subdued text to reduce emphasis independent of font size and weight.</p>
  <p class="mrk-text-body-sm"><strong>.mrk-text-subdued</strong></p>
</div>

<div>
  <p><strong>Use strong text to increase emphasis independent of font size and color.</strong></p>  <p class="mrk-text-body-sm"><strong>Use <code>&lt;strong&gt;</code> on body text</strong></p>
</div>

{% call code.sample() %}
<p class="mrk-text-subdued">Use subdued text to reduce emphasis independent of font size and weight.</p>
<p><strong>Use strong text to increase emphasis independent of font size and color.</strong></p> 
{% endcall %}

## Centered Text

Use `.mrk-text-center` to align text to the center of a container.

**Example**  
A block of text with aligned to the center.

<div class="doc-example">
  <p class="mrk-text-center">Thank you for your attention.</p>
</div>

{% call code.sample() %}
<p class="mrk-text-center">Thank you for your attention.</p>
{% endcall %}

## Columns

Use `.mrk-columns` to distribute multiple lines of text into two or more columns. Use custom properties to override the value of the number of columns and the column width. 

You can override the default values for the number of columns and space between columns using custom properties.

<table class="doc-table">
  <tr>
    <th>Custom Property</th>
    <th>Default Value</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><code>--columns</code></td>
    <td>2</td>
    <td>Number of columns</td>
  </tr>
  <tr>
    <td><code>--gap</code></td>
    <td>60px</td>
    <td>Space between columns</td>
  </tr>
</table>

**Example**  
Text divided into columns.

<div class="doc-example">
  <p class="mrk-columns" style="--columns: 3; --gap: 30px">
    HTML/CSS<br>
    JavaScript<br>
    Version Control/Git<br>
    Backend Development<br>
    Databases<br>
    Web Hosting/Deployment<br>
    Testing<br>
    API Development & Integration<br>
    Security Best Practices<br>
    Responsive and Mobile Design<br>
    Frontend<br>
    Backend<br>
    Frameworks & Libraries<br>
    Database Technologies<br>
    Version Control & Collaboration<br>
    Build Tools & Package Managers<br>
    DevOps & Deployment<br>
    APIs<br>
    Content Management Systems (CMS)<br>
    Problem-Solving<br>
    Attention to Detail<br>
    Communication<br>
    Team Collaboration<br>
    Time Management<br>
    Continuous Learning
  </p>
</div>

{% call code.sample() %}
<p class="mrk-columns" style="--columns: 3; --gap: 30px">
  HTML/CSS<br>
  JavaScript<br>
  Version Control/Git<br>
  ...
  Team Collaboration<br>
  Time Management<br>
  Continuous Learning
</p>
{% endcall %}