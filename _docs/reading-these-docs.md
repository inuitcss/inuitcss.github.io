---
layout: page
title: "Reading These Docs"
group: introduction
page-class: c-page--docs
has-sub-content: true
sub-content: docs
---

Anything that is mandatory is written plainly, e.g.:

```
class="o-layout"
```

Anything that is mandatory but requires user input is written inside of `&lt;`,
e.g.:

```
class="o-layout__item <width>"
```

Anything that is optional is written inside of `[]`, e.g.:

```
class="o-layout--[options]"
```

All together, that might look a little like this:

```
<div class="o-layout  [o-layout--<options>]">
  <div class="o-layout__item  <width>">
    ...
  </div>
</div>
```
