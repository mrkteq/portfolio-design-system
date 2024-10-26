---
title: Single Page
eleventyNavigation:
  key: Single Page
  parent: Layouts
  order: 1
---

{% import 'macros/code.njk' as code %}

<style>
  .mrk-layout-single-page-sample {
    border: 1px solid #615384;
    background-color: #151515ff;
    display: grid;
    grid-template-columns: 64px 1fr 2fr 64px;
    grid-template-rows: 1fr 1fr 1fr 1fr 140px;
    > * {
      outline: 1px dashed darkslateblue;
      outline-offset: 0px;
      padding: .5rem 1rem;
    }
    > [data-grid-area="home"] {
      grid-column: 1 / -1;
      grid-row: 1 / 2;
      aspect-ratio: 1200/567;
      background-color: #CBDBE3;
    }
    > [data-grid-area="home-content"] {
      grid-column: 2 / 4;
      grid-row: 1 / 2;
      aspect-ratio: 180/30;
      background-color: #CBDBE3;
      align-self: center;
      filter: brightness(0.9);
      margin: 1rem;
    }
    > [data-grid-area="about"] {
      grid-column: 1 / -1;
      grid-row: 2 / 3;
      aspect-ratio: 1200/567;
      background-color: #CBDBE3;
    }
    > [data-grid-area="about-content-a"] {
      grid-column: 2 / 3;
      grid-row: 2 / 3;
      aspect-ratio: 50/50;
      background-color: #CBDBE3;
      align-self: center;
      filter: brightness(0.9);
      margin: 1rem;
    }
    > [data-grid-area="about-content-b"] {
      grid-column: 3 / 4;
      grid-row: 2 / 3;
      aspect-ratio: 46/20;
      background-color: #CBDBE3;
      align-self: center;
      filter: brightness(0.9);
      margin: 1rem;
    }
    > [data-grid-area="projects"] {
      grid-column: 1 / -1;
      grid-row: 3 / 4;
      aspect-ratio: 1200/567;
      background-color: #CBDBE3;
    }
    > [data-grid-area="projects-content-a"] {
      grid-column: 2 / 3;
      grid-row: 3 / 4;
      aspect-ratio: 50/50;
      background-color: #CBDBE3;
      filter: brightness(0.9);
      align-self: center;
      margin: 1rem;
    }
    > [data-grid-area="projects-content-b"] {
      grid-column: 3 / 4;
      grid-row: 3 / 4;
      aspect-ratio: 46/20;
      background-color: #CBDBE3;
      filter: brightness(0.9);
      align-self: center;
      margin: 1rem;
    }
    > [data-grid-area="contact"] {
      grid-column: 1 / -1;
      grid-row: 4 / 5;
      aspect-ratio: 1200/567;
      background-color: #CBDBE3;
    }
    > [data-grid-area="contact-content"] {
      grid-column: 2 / 4;
      grid-row: 4 / 5;
      aspect-ratio: 180/30;
      background-color: #CBDBE3;
      align-self: center;
      filter: brightness(0.9);
      margin: 1rem;
    }
    > [data-grid-area="links"] {
      grid-column: 1 / -1;
      grid-row: 5 / 6;
      background-color: #CBDBE3;
    }
    > [data-grid-area="links-content"] {
      grid-column: 2 / 4;
      grid-row: 5 / 6;
      aspect-ratio: 180/30;
      background-color: #CBDBE3;
      align-self: end;
      filter: brightness(0.9);
      margin: 1rem;
    }
  }
</style>

The Single Page layout features several overlapping elements.

* The **Home** section will always feature something cool.It can have a background image by simply passing in the image URL with the custom property `--image`, or a background color or gradient. 
* The **About** section is a very short summary of me as i see me and who i am.
* The **Projects** section is a dynamic loop that displays all of my projects and shows links to the source code and live url.
* The **Contact** section is a short, friendly and honest call to action.
* The **Links** section is the footer and basically contains links to where i can be found on the web and anything else.

**Example**  
A visualization of the Home section layout. (Areas are not to scale.)

<div class="mrk-layout-single-page-sample">
  <section data-grid-area="home">Home</section>
  <div data-grid-area="home-content"></div>

  <section data-grid-area="about">About</section>
  <div data-grid-area="about-content-a"></div>
  <div data-grid-area="about-content-b"></div>

  <section data-grid-area="projects">Projects</section>
  <div data-grid-area="projects-content-a"></div>
  <div data-grid-area="projects-content-b"></div>

  <section data-grid-area="contact">Contact</section>
  <div data-grid-area="contact-content"></div>

  <section data-grid-area="links">Links</section>
  <div data-grid-area="links-content"></div>
</div>

{% call code.sample() %}
<div class="mrk-layout-single-page-sample">
  <section data-grid-area="home" style="--image: url('hero.jpg')"></section>
  <section data-grid-area="about"></section>
  <section data-grid-area="projects"></section>
  <section data-grid-area="contact"></section>
  <section data-grid-area="links"></section>
</div>
{% endcall %}