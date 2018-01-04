---
layout: page
title: "Font-size"
group: tools
page-class: c-page--docs
has-sub-content: true
sub-content: docs
filename: "_tools.font-size.scss"
---

{% include file-info.html %}

Create a fully formed type style (sizing and vertical rhythm) by passing in a
single value, e.g.:

    .usage {
      @include inuit-font-size(12px);
    }

This will generate a rem-based font-size, a `px` fallback for older browsers, as well as a unitless line-height
which will place the element on your baseline, e.g.:

    // CSS
    .usage {
      font-size: 12px;
      font-size: 0.75rem;
      line-height: 2;
    }

If you do not want to generate a line-height automatically, you
simply pass in your own value as a second paramater:

    .usage {
      @include inuit-font-size(12px, 1.5);
    }

This will yield:

    // CSS
    .usage {
      font-size: 12px;
      font-size: 0.75rem;
      line-height: 1.5;
    }

This parameter can be any integer, `inherit`, or `normal`. If you don't want
a line-height at all, pass in a second paramater of `false` or `"none"`:

    .usage {
      @include inuit-font-size(12px, false);
    }

This will yield:

    // CSS
    .usage {
      font-size: 12px;
      font-size: 0.75rem;
    }

There may be situations where the generated declarations of the mixin need to carry an `!important` (e.g. when you are using the mixin in the utilities layer). In this case you can just pass `$important: true` as last parameter in the mixin call:

    .usage {
      @include inuit-font-size(12px, $important: true);
    }

    // CSS
    .usage {
      font-size: 12px !important;
      font-size: 0.75rem !important;
      line-height: 2 !important;
    }



## Mixins

    .usage {
      @include inuit-font-size(<px-value>, [line-height], [$important: true]);
    }
