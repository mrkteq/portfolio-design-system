---
title: Slider
eleventyNavigation:
  key: Slider
  parent: Components
  order: 4
---

{% import 'macros/code.njk' as code %}

## Certificates

Used to show a collection of certificates on a page.

**Example**  
Certificates.

<div class="doc-example">
  <div class="custom-slider">
    <div class="custom-slider__container">
      <div class="custom-slider__slide">
        <img 
          src="/assets/images/certificates/certificate-of-completion-for-complete-python-developer-in-2020-zero-to-mastery.jpg" 
          alt="Slide 1"
          class="custom-slider__image"
          loading="lazy"
        >
      </div>
      <div class="custom-slider__slide">
        <img 
          src="/assets/images/certificates/certificate-of-completion-for-complete-web-developer-in-2020-zero-to-mastery.jpg" 
          alt="Slide 2"
          class="custom-slider__image"
          loading="lazy"
        >
      </div>
      <div class="custom-slider__slide">
        <img 
          src="/assets/images/certificates/certificate-of-completion-for-future-of-a-i-how-to-use-chatgpt.jpg" 
          alt="Slide 3"
          class="custom-slider__image"
          loading="lazy"
        >
      </div>
      <div class="custom-slider__slide">
        <img 
          src="/assets/images/certificates/chatgpt-large-language-models-llms-a-practical-guide.jpg" 
          alt="Slide 4"
          class="custom-slider__image"
          loading="lazy"
        >
      </div>
      <div class="custom-slider__slide">
        <img 
          src="/assets/images/certificates/the-complete-career-toolkit.jpg" 
          alt="Slide 5"
          class="custom-slider__image"
          loading="lazy"
        >
      </div>
    </div>
  </div>

{% call code.sample() %}
<div class="custom-slider">
  <div class="custom-slider__container">
    <div class="custom-slider__slide">
      <img 
        src="/assets/images/certificates/certificate-of-completion-for-complete-python-developer-in-2020-zero-to-mastery.jpg" 
        alt="Slide 1"
        class="custom-slider__image"
        loading="lazy"
      >
    </div>
    <div class="custom-slider__slide">
      <img 
        src="/assets/images/certificates/certificate-of-completion-for-complete-web-developer-in-2020-zero-to-mastery.jpg" 
        alt="Slide 2"
        class="custom-slider__image"
        loading="lazy"
      >
    </div>
    <div class="custom-slider__slide">
      <img 
        src="/assets/images/certificates/certificate-of-completion-for-future-of-a-i-how-to-use-chatgpt.jpg" 
        alt="Slide 3"
        class="custom-slider__image"
        loading="lazy"
      >
    </div>
    <div class="custom-slider__slide">
      <img 
        src="/assets/images/certificates/chatgpt-large-language-models-llms-a-practical-guide.jpg" 
        alt="Slide 4"
        class="custom-slider__image"
        loading="lazy"
      >
    </div>
    <div class="custom-slider__slide">
      <img 
        src="/assets/images/certificates/the-complete-career-toolkit.jpg" 
        alt="Slide 5"
        class="custom-slider__image"
        loading="lazy"
      >
    </div>
  </div>
</div>
{% endcall %}

## Cover Flow

Used to show a navigable and dynamically generated stack of cards on a page.

**Example**  
The Image Gallery.

<div class="doc-example">
<div class="custom-slider">
  <div class="custom-slider__container">
    <div class="custom-slider__slide">
    <img 
        src="/assets/images/screens/argyll-lg.jpeg" 
        alt="Slide 1"
        class="custom-slider__image"
        loading="lazy"
    >
    </div>
    <div class="custom-slider__slide">
    <img 
        src="/assets/images/screens/bridle-lg.jpeg" 
        alt="Slide 2"
        class="custom-slider__image"
        loading="lazy"
    >
    </div>
    <div class="custom-slider__slide">
    <img 
        src="/assets/images/screens/newcastle-lg.jpeg" 
        alt="Slide 3"
        class="custom-slider__image"
        loading="lazy"
    >
    </div>
  </div>
</div>
</div>

{% call code.sample() %}
<div class="custom-slider">
  <div class="custom-slider__container">
    <div class="custom-slider__slide">
    <img 
        src="/assets/images/screens/argyll-lg.jpeg" 
        alt="Slide 1"
        class="custom-slider__image"
        loading="lazy"
    >
    </div>
    <div class="custom-slider__slide">
    <img 
        src="/assets/images/screens/bridle-lg.jpeg" 
        alt="Slide 2"
        class="custom-slider__image"
        loading="lazy"
    >
    </div>
    <div class="custom-slider__slide">
    <img 
        src="/assets/images/screens/newcastle-lg.jpeg" 
        alt="Slide 3"
        class="custom-slider__image"
        loading="lazy"
    >
    </div>
</div>
{% endcall %}