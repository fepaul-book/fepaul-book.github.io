---
layout: page
title: ReadMyBook
description: Ai-based app with text recognition for reading a children’s book aloud.
img: assets/img/readmybook-cover.jpg
importance: 3
category: programming
---


<video width="640" height="240" controls autoplay>
  <source src="/assets/video/book-presentation.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>


The app has been developed as a complement to a children's book by a private friend of mine. The goal of the app is to enable children, especially those with busy parents, to have children's books read to them. The app allows children to independently get the book read aloud from a specific page by scanning it. By scanning designated stickers, users can choose between three reading modes.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/autorin-liest.png" title="Autor liest vor" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Eltern-lesen.png" title="Eltern lesen vor" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/nachtmodus.png" title="Nachtmodus" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
1. The audio recorded by the author is played.
2. The audio recorded by the parents is played.
3. The audio recorded by the author, with audio description (including image descriptions), is played.
</div>


Parents have the option to record their own audios and set page transitions, ensuring that in this mode, reading starts from the correct page.

Besides recognizing the correct page through text recognition, users can also navigate to the right page using button controls.

The app utilizes the text recognition feature of Android's ML Kit. The designs of the buttons and graphics were created by Klarissa Okfen.

In the following graphic, the functionality of the app is briefly explained in German.
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/readmybook-description.jpg" title="readmybook app description" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    This is a brief description of the app's functionality in German.
</div>
