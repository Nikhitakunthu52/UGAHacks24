---
title: Find Missing Children
nav: Search
description: >
    Search for Missing Children here.
---

## Missing Children


{% capture text %}
1. Call 489-567-8235 
2. A 5' 2" tall, golden-brown skinned woman, light brown eyes, angled lips and a square jaw. She has coiled, grey hair, has a chipped tooth. She was last seen carrying a book.
3. [Last Seen Location](https://www.google.com/maps/place/44%C2%B049'46.5%22N+122%C2%B047'40.3%22W/@44.82957,-122.79453,17950m/data=!3m1!1e3!4m4!3m3!8m2!3d44.82957!4d-122.79453?entry=ttu).
{% endcapture %}
{% include card.html text=text header="Aava Ebba" title="Last Seen 12-3-2022" img="uidaho-workshop.jpg" %}


## Components Includes

`workshop-template-b` contains a series of [Liquid "includes"](https://jekyllrb.com/docs/includes/) to simplify adding basic [Bootstrap 5 components](https://getbootstrap.com/docs/5.0/components/) to your Markdown content.
The includes can be found in the "_includes" folder. 
Check the comments at the top of each include file for details about options and how to use them.

Examples below demonstrate the includes with sample include `code` followed by the rendered feature:

--------

### Figures 

- put any images you want to use in the "images" folder, or use a full URL to external images.
- in the markdown file where you want the image to appear, use the `figure.html` include on its own line, following the pattern: `{% raw %}{% include figure.html img="my-cat.jpg" alt="cat" caption="My cat" width="50%" %}{% endraw %}`
- figures will be centered, and can optionally be given a caption and percentage width.

Include code: 

`{% raw %}{% include figure.html img="uidaho-workshop.jpg" alt="workshop scene" caption="Library workshops!" width="75%" %}{% endraw %}`

Becomes:

{% include figure.html img="uidaho-workshop.jpg" alt="workshop scene" caption="Library workshops!" width="75%" %}

----------

### Alerts

Include code:

`{% raw %}{% include alert.html text="This is a Bootstrap [Alert](https://getbootstrap.com/docs/4.1/components/alerts/)" align="center" color="success" %}{% endraw %}`

Becomes:

{% include alert.html text="This is a [Bootstrap Alert](https://getbootstrap.com/docs/4.1/components/alerts/)" align="center" color="success" %}

-----------

### Link Buttons 

Include code:

`{% raw %}{% include button.html text="Bootstrap Docs" link="https://getbootstrap.com/docs/5.1/components/buttons/" color="info" %}{% endraw %}`

Becomes:

{% include button.html text="Bootstrap Docs" link="https://getbootstrap.com/docs/5.1/components/buttons/" color="info" %}

---------

### Cards

Include code:

```{% raw %}
{% capture text %}
1. Can add more complex text using markdown.
2. Use a Liquid capture to create the text.
3. It magically becomes a [Bootstrap Card](https://getbootstrap.com/docs/4.1/components/card/).
{% endcapture %}
{% include card.html text=text header="Example Card" title="Title example" img="uidaho-workshop.jpg" %}{% endraw %}
```

Becomes: 

{% capture text %}
1. Can add more complex text using markdown.
2. Use a Liquid capture to create the text.
3. It magically becomes a [Bootstrap Card](https://getbootstrap.com/docs/4.1/components/card/).
{% endcapture %}
{% include card.html text=text header="Example Card" title="Title example" img="uidaho-workshop.jpg" %}

------------

### Accordion

Include code:

`{% raw %}{% include accordion.html title1="Example section" text1=example1 title2="Section two" text2=example2 title3="Section three" text3=example3 %}{% endraw %}`

Becomes:

{% include accordion.html title1="Section one" text1="Some text content" title2="Section two" text2="Some text content" title3="Section three" text3="Some text content" %}

------------

### Modal

Include code:

`{% raw %}{% include modal.html button="Try Me" color="success" title="Example Modal" text="This is a modal, with little text." %}{% endraw %}`

Becomes:

{% include modal.html button="Try Me" color="success" title="Example Modal" text="This is a modal, with little text." %}

-------------

### YouTube embed

Include code:

`{% raw %}{% include video-embed.html youtubeid="moJgWrD6dwg" caption="Example video" %}{% endraw %}`

Becomes:

{% include video-embed.html youtubeid="moJgWrD6dwg" caption="Example video" %}

-------------

### Jumbotron

Include code:

`{% raw %}{% include jumbotron.html heading="Jumbotron Include" text="Paragraph content goes here." button-text="Learn more" button-color="outline-primary" button-link="https://github.com/evanwill/workshop-template-b" border=true %}{% endraw %}`

Becomes: 

{% include jumbotron.html heading="Jumbotron Include" text="Paragraph content goes here." button-text="Learn more" button-color="outline-primary" button-link="https://github.com/evanwill/workshop-template-b" border=true %}
