---
layout: page
title: "Media object"
group: objects
page-class: c-page--docs
has-sub-content: true
sub-content: docs
filename: "_objects.media.scss"
demo: "media"
classes: [
    "o-media",
    "o-media--tiny",
    "o-media--small",
    "o-media--large",
    "o-media--huge",
    "o-media--flush",
    "o-media--reverse"
]
---

[DEPENDENCIES?]

[VARS?]

{% include file-info.html %}

{% include class-list.html %}

The Media object is inuitcss’ implementation of [Nicole
Sullivan](https://twitter.com/stubbornella)’s <cite>media object</cite>—the
poster child of OOCSS. To find out where it all started, read [Nicole’s blog
post](http://www.stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code/).


## Usage

Basic usage of the Media object uses the required classes:

    <div class="o-media">
        <img class="o-media__img" src="/path/to/image.png" alt="" />
        <div class="o-media__body">
            <p>Text-like content goes here.</p>
        </div>
    </div>

The only valid children of the `.o-media` node are `.o-media__img` and
`.o-media__body`.

{% include demo-iframe.html %}
