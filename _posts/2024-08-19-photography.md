---
layout: post
title: An introduction to photography
date: 2024-08-19 00:00:00
description: Capturing the marvels of the world
tags: photography hobbies
categories: free-time
featured: false
related_posts: true
giscus_comments: true
thumbnail: assets/img/photography_introduction/wide_earth.jpeg
images:
  compare: true
  slider: true
---

### Smartphone transition

<p>I have recently acquired a new smartphone, the iPhone 15 Pro. My last one was the iPhone 6S Plus, so it was a pretty big change. Not only in power, but in camera capabilities. This is even more evident if your old phone's camera does not focus on any object or area.</p>

<p>Photography hasn't been a big interest of mine, or at least investing time in it was something I rarely considered. I would occasionally find amazing images shared in the internet of different places, moments, landscapes... Some of them very pleasant to observe. Why not create my own? Well, I never had the tools to begin with. But I gave it a shot recently.</p>

<p style="margin-bottom:1cm;"></p>


### The first picture

<p>I went on a trip to Furnas in my home island São Miguel with my parents and grandma. We ate breakfast there in the silence of the morning by the lake. This was my first proper picture with the phone:</p>

<img-comparison-slider>
  {% include figure.liquid path="assets/img/photography_introduction/furnas_unedited.jpeg" title="Morning by the Furnas' lake unedited" class="img-fluid rounded z-depth-1" slot="first" %}
  {% include figure.liquid path="assets/img/photography_introduction/furnas.jpeg" title="Morning by the Furnas edited' lake" class="img-fluid rounded z-depth-1" slot="second" %}
</img-comparison-slider>
<div class="caption">
Morning by the Furnas' lake
</div>

<p>I explored a few of the editing functionalities the iPhone provides in the camera app and tried to make the image more pleasant. My main idea with the editing on this one was to make it feel like a calm morning, vegetation standing out with some humidity and vibrant but realistic colors, and displaying a clear blue sky. I believe it was a good result. Nonetheless, it was a first attempt at editing.</p>

One of the key aspects I learned through this is that too much editing may be doing exactly what you want in general, but the image may lose detail in some areas. This is not optimal, unless it isn't noticeable. The bushes are the main object affected by the editing in negative terms, losing some detail to darker tones. However, it gives the impression that the tree's shadow has some influence in the matter.

Below is a brief description of every functionality I explored[^1].

**Light controls:**
<ul>
  <li>Exposure - act as though more or less light got into the lens</li>
  <li>Brilliance - lighten shadows while toning down highlights</li>
  <li>Highlights - adjust the brightness of the lightest parts in the image</li>
  <li>Shadows - adjust the brightness of the darkest parts in the image</li>
  <li>Contrast - make the darker parts darker and the lighter parts lighter</li>
  <li>Brightness - make the entire image lighter or darker</li>
  <li>Black point - adjust the very darkest part of the image</li>
</ul>

**Color controls:**
<ul>
  <li>Saturation - change the intensity of colors in the image</li>
  <li>Vibrancy - change the intensity of the least saturated colors</li>
  <li>Warmth - adjust the yellow and blue tones to warm or cool an image.</li>
  <li>Tint - adjust the green or magenta tones in your image</li>
</ul>

**Detail controls:**
<ul>
  <li>Sharpness - sharpen the edges in your image</li>
  <li>Definition - make the details in your image clearer</li>
  <li>Noise reduction - reduce the graininess in your image</li>
  <li>Vignette - darken the corners of the image</li>
</ul>

**Additional editing features:**
<ul>
  <li>Rotation</li>
  <li>Crop</li>
</ul>

<p style="margin-bottom:1cm;"></p>


### Testing the lenses

After having lunch at _Ponta do Garajau_ restaurant, in Ribeira Quente, we also visited the Santa Iria viewpoint. A sort of small peninsula stands out from the entire view. I felt this was perfect to test out the different lenses. Here are the results for the wide camera, 24mm lenses, 28mm lenses and 35 mm lenses, post-editing:

<swiper-container keyboard="true" navigation="true" pagination="false" rewind="true">
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/photography_introduction/wide_earth.jpeg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/photography_introduction/24_earth.jpeg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/photography_introduction/28_earth.jpeg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/photography_introduction/35_earth.jpeg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
</swiper-container>
<div class="caption">
Santa Iria viewpoint
</div>

This should be fairly obvious to some people, but the higher the focal length, the closer the image appears to be taken. Additionally, it seems that more detail is preserved from objects at further distances.

<div id="mapContainer" style="width: 100%; height: 400px;"></div>

<script src="https://js.api.here.com/v3/3.1/mapsjs-core.js"></script>
<script src="https://js.api.here.com/v3/3.1/mapsjs-service.js"></script>
<script src="https://js.api.here.com/v3/3.1/mapsjs-ui.js"></script>
<script src="https://js.api.here.com/v3/3.1/mapsjs-mapevents.js"></script>
<link rel="stylesheet" type="text/css" href="https://js.api.here.com/v3/3.1/mapsjs-ui.css" />

<script>
    // Replace 'YOUR_API_KEY' with your actual HERE API key
    var platform = new H.service.Platform({
        apikey: 'XS0cL8OT4rvzhAkhaEWK6gMK0M97Oxxxc4cpxgB7CpI'
    });

    // Obtain the default map types from the platform object:
    var maptypes = platform.createDefaultLayers();

    // Instantiate (and display) a map object:
    var map = new H.Map(
        document.getElementById('mapContainer'),
        maptypes.raster.satellite.map, // This can be changed to satellite or hybrid
        {
            zoom: 13.05,
            center: { lat: 37.824, lng: -25.462 }
        });

    // Enable the event system on the map instance:
    var mapEvents = new H.mapevents.MapEvents(map);

    // Instantiate the default behavior, providing pan/zoom capabilities:
    var behavior = new H.mapevents.Behavior(mapEvents);

    // Create the default UI:
    var ui = H.ui.UI.createDefault(map, maptypes);
</script>
<div class="caption">
Santa Iria viewpoint location
</div>



<p style="margin-bottom:1cm;"></p>


### Portrait mode

One more feature that was left more me to test was the portrait mode. I decided to test it on a small wooden plane that I have since I was a kid and that I love to use as decoration. Here is the result:

<img-comparison-slider>
  {% include figure.liquid path="assets/img/photography_introduction/plane_unedited.jpeg" title="Wooden plane unedited" class="img-fluid rounded z-depth-1" slot="first" %}
  {% include figure.liquid path="assets/img/photography_introduction/plane.jpeg" title="Wooden plane" class="img-fluid rounded z-depth-1" slot="second" %}
</img-comparison-slider>
<div class="caption">
Wooden plane
</div>

It is interesting to point out that a random hair was captured in this picture. The camera can preserve so much detail at a close distance that one of the smallest things the human eye can see can be captured.

<p style="margin-bottom:1cm;"></p>


### Rooftop experiences

On one day, I captured the city from a rooftop. During the entire day, the sky was very clear, so it allowed for some amazing pictures. I took one on sunrise and one in the beginning of the night. The night picture was very tricky to edit since the camera was not exposed to a lot of light, even though it was full moon. I did my best to make it a decently looking image, but I feel like it still was not enough. Equipment will only take you so far.

<swiper-container keyboard="true" navigation="true" pagination="false" rewind="true">
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/photography_introduction/roof.jpeg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
  <swiper-slide>{% include figure.liquid loading="eager" path="assets/img/photography_introduction/roof_night.jpeg" class="img-fluid rounded z-depth-1" %}</swiper-slide>
</swiper-container>
<div class="caption">
Rooftop experiences
</div>


_Lourenço_

##### <b>References</b>

[^1]: <a href="https://appletoolbox.com/editing-photos-iphone/">https://appletoolbox.com/editing-photos-iphone/</a> [accessed 20/08/2024]