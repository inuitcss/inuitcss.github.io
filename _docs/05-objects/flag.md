---
title: "Flag object"
group: "Objects"
filename: "_objects.flag.scss"
requirement: optional
order: 7
---

{% include file-info.html %}

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
