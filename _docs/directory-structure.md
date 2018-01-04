---
layout: page
title: "Directory Structure"
group: getting-started
page-class: c-page--docs
has-sub-content: true
sub-content: docs
---

inuitcss follows a specific folder structure, which you should follow as well in your own CSS directory:

* `/settings`: Global variables, site-wide settings, config switches, etc.
* `/tools`: Site-wide mixins and functions.
* `/generic`: Low-specificity, far-reaching rulesets (e.g. resets).
* `/elements`: Unclassed HTML elements (e.g. `a {}`, `blockquote {}`, `address {}`).
* `/objects`: Objects, abstractions, and design patterns (e.g. `.o-layout {}`).
* `/components`: Discrete, complete chunks of UI (e.g. `.c-carousel {}`). This is the one layer that inuitcss doesn’t provide code for, as this is completely your terrain.
* `/utilities`: High-specificity, very explicit selectors. Overrides and helper
  classes (e.g. `.u-hidden {}`).

Following this structure allows you to intersperse inuitcss’ code with your own, so that your `main.scss` file might look something like this:

```scss
// SETTINGS
@import "settings/settings.config";
@import "node_modules/inuitcss/settings/settings.core";
@import "settings/settings.global";
@import "settings/settings.colors";

// TOOLS
@import "node_modules/inuitcss/tools/tools.font-size";
@import "node_modules/inuitcss/tools/tools.clearfix";
@import "node_modules/sass-mq/mq";
@import "tools/tools.aliases";

// GENERIC
@import "node_modules/inuitcss/generic/generic.box-sizing";
@import "node_modules/inuitcss/generic/generic.normalize";
@import "node_modules/inuitcss/generic/generic.shared";

// ELEMENTS
@import "node_modules/inuitcss/elements/elements.page";
@import "node_modules/inuitcss/elements/elements.headings";
@import "elements/elements.links";
@import "elements/elements.quotes";

// OBJECTS
@import "node_modules/inuitcss/objects/objects.layout";
@import "node_modules/inuitcss/objects/objects.media";
@import "node_modules/inuitcss/objects/objects.flag";
@import "node_modules/inuitcss/objects/objects.list-bare";
@import "node_modules/inuitcss/objects/objects.list-inline";
@import "node_modules/inuitcss/objects/objects.box";
@import "node_modules/inuitcss/objects/objects.block";
@import "node_modules/inuitcss/objects/objects.tables";

// COMPONENTS
@import "components/components.buttons";
@import "components/components.page-head";
@import "components/components.page-foot";
@import "components/components.site-nav";
@import "components/components.ads";
@import "components/components.promo";

// UTILITIES
@import "node_modules/inuitcss/utilities/utilities.widths";
@import "node_modules/inuitcss/utilities/utilities.headings";
@import "node_modules/inuitcss/utilities/utilities.spacings";
```

**NOTE:** Every `@import` above which begins with "node_modules" is inuitcss core. When you installed inuitcss via bower, these imports would begin with "bower_components".

Having your own and inuitcss’ partials interlaced like this is one of the real strengths of inuitcss.
