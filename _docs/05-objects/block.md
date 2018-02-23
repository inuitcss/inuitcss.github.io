---
title: "Block object"
group: "Objects"
filename: "_objects.block.scss"
requirement: optional
order: 30
---

{% include file-info.html %}

When you want to stack an image on top of a block of text, this object is what you need.

## Usage

The basic markup structure is as follows:

    <div class="o-block">
      <div class="o-block__img">
        <img src="/path/to/image.png">
      </div>
      <div class="o-block__body">
        Text-like content goes here.
      </div>
    </div>

The only valid children of the `.o-block` node are `.o-block__img` and
`.o-block__body`.

## Default block object

The default variant of the block object includes a spacing equal the amount of `$inuit-global-spacing-unit` between the image and the content.

{% include demo.html variant="block" %}

## Spacing variants

If you want to change the spacing between the image and the content, you can vary this by adding any of the following additional modifier classes:

### `.o-block--tiny`
{% include demo.html variant="block--tiny" %}

### `.o-block--small`
{% include demo.html variant="block--small" %}

### `.o-block--large`
{% include demo.html variant="block--large" %}

### `.o-block--huge`
{% include demo.html variant="block--huge" %}

### `.o-block--flush`
{% include demo.html variant="block--flush" %}

## Alignment variants

You can align the image and the content either to the left or to the right by adding the respective additional modifier class:

### `.o-block--right`
{% include demo.html variant="block--right" %}

### `.o-block--left`
{% include demo.html variant="block--left" %}
