---
title: "Core"
group: "Settings"
filename: "_settings.core.scss"
permalink: /docs/settings/core/
requirement: required
order: 1
---

{% include file-info.html %}

Although it might not look like that, but this is probably the most important file of the whole framework. It provides some really far-reaching Sass variables which—when altered—can change the look of your application massivley. That's why you should determine the values of the variables right at the beginning of your project.

The two most important variables are:

    $inuit-global-font-size:    16px !default;
    $inuit-global-line-height:  24px !default;

The following is very important:

    $inuit-global-spacing-unit: round($inuit-global-line-height) !default;

Probably the most opinionated thing inuitcss will ever do is reassign your `$inuit-global-line-height` variable to `$inuit-global-spacing-unit`. This value then becomes the cornerstone of your UI, acting as the default margin and padding value for any components that require it.

While this might seem overly opinionated, it does mean that:

1. **You get a free vertical rhythm** because everything sits on a multiple of your baseline, and…
2. **We reduce the amount of [magic numbers](http://csswizardry.com/2012/11/code-smells-in-css/#magic-numbers) in our codebase** because we can rationalise where the majority of values in our CSS came from.

On top of `$inuit-global-spacing-unit` as base spacing variable, you also get four variants to use for spacings:

* `$inuit-global-spacing-unit-tiny`
* `$inuit-global-spacing-unit-small`
* `$inuit-global-spacing-unit-large`
* `$inuit-global-spacing-unit-huge`

They all depend on `$inuit-global-spacing-unit` regarding their values, but you can control the factor in which they alter from the base spacing by overriding their value:

    $inuit-global-spacing-unit-factor-tiny:   0.25 !default;
    $inuit-global-spacing-unit-factor-small:  0.5  !default;
    $inuit-global-spacing-unit-factor-large:  2    !default;
    $inuit-global-spacing-unit-factor-huge:   4    !default;

## Variables

    // The basic font-size for your whole site
    $inuit-global-font-size

    // The basic line-height for your whole site
    $inuit-global-line-height

    // A base spacing variable for your whole project
    $inuit-global-spacing-unit

    // Sizing variants for spacings
    $inuit-global-spacing-unit-tiny
    $inuit-global-spacing-unit-small
    $inuit-global-spacing-unit-large
    $inuit-global-spacing-unit-huge

    // Controls the factor in which the sizing
    // variants differ from the base spacing
    $inuit-global-spacing-unit-factor-tiny
    $inuit-global-spacing-unit-factor-small
    $inuit-global-spacing-unit-factor-large
    $inuit-global-spacing-unit-factor-huge

