---
layout: page
title: "Core"
group: settings
page-class: c-page--docs
has-sub-content: true
sub-content: docs
filename: "_settings.core.scss"
---

{% include file-info.html %}

This is probably the most important file of the whole framework. It provides some really far-reaching Sass variables which—when altered—can change the look of your application massivley. That's why you should determine the values of the variables right at the beginning of your project.

The two most important variables are:

    $inuit-global-font-size:    16px !default;
    $inuit-global-line-height:  24px !default;

The following is very important:

    $inuit-global-spacing-unit: round($inuit-global-line-height) !default;

What this does is reassigning the global line-height to a multipurpose spacing variable
