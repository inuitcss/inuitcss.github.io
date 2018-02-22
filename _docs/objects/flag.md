---
layout: page
title: "Flag object"
group: objects
page-class: c-page--docs
has-sub-content: true
sub-content: docs
filename: "_objects.flag.scss"
requirement: optional
demo: "flag"
classes: [
    "o-flag",
    "o-flag--tiny",
    "o-flag--small",
    "o-flag--large",
    "o-flag--huge",
    "o-flag--flush",
    "o-flag--reverse",
    "o-flag--top",
    "o-flag--bottom"
]
---

{% include file-info.html %}

{% include class-list.html %}

The `flag` object module is an object similar in appearance to [the media
object](https://github.com/inuitcss/objects.media), but which provides slightly
more advanced functionality.


## Usage

Basic usage of the Flag object uses the required classes:

    <div class="o-flag">
        <div class="o-flag__img">
            <img src="/path/to/image.png" alt="" />
        </div>
        <div class="o-flag__body">
            <p>Text-like content goes here.</p>
        </div>
    </div>

The only valid children of the `.o-flag` node are `.o-flag__img` and
`.o-flag__body`.

{% include demo-iframe.html %}
