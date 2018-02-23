---
title: "Modifying inuitcss"
group: "Getting Started"
order: 20
---

inuitcss is highly configurable, but **should not be edited directly**. The correct way to make changes to inuitcss is to pass in variables **before** you `@import` the specific file.

Let’s take [`settings.core`](https://github.com/inuitcss/inuitcss/blob/develop/settings/_settings.core.scss) as an example. In this file we can see the variables `$inuit-global-font-size` and `$inuit-global-line-height`. If we want to keep these as-is then we needn’t do anything other than `@import` the file. If we wanted to change these values to `12px` and `18px` respectively (don’t worry, inuitcss will convert these pixel values to `rem` values for you), then we just need to pass those values in **before** the `@import`, thus:

```scss
$inuit-global-font-size:   12px;
$inuit-global-line-height: 18px;
@import "node_modules/inuitcss/settings/settings.core";
```

The same goes for any inuitcss module: you can configure it by predefining any
of its variables immediately **before** the `@import`:

```scss
$inuit-wrapper-width: 1480px;
@import "node_modules/inuitcss/objects/objects.wrapper";

$inuit-fractions: 1 2 3 4 12;
@import "node_modules/inuitcss/utilities/utilities.widths";
```

This method of modifying the framework means that you don’t need to edit any
files directly (thus making it easier to update the framework), but also means
that you’re not left with huge, bloated, monolithic variables files from which
you need to configure an entire library.

## Extending inuitcss

To extend inuitcss with your own code, simply create a partial in the `<section>.<file>` format, put it into the
[appropriate directory](/docs/directory-structure/) and `@import` it in your `main.scss`.

But extending inuitcss does not only mean adding your own partials to the project. Due to inuitcss’ modular nature, you can also _omit_ those partials of inuitcss you don't need. But be aware that there are a few interdependencies between various inuitcss partials. The only partial that is indispensable for the framework to work properly is `settings.core`, though. But we recommend using all partials from the `/settings`, `/tools` and `/generic` layer.
