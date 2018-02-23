---
title: "Setup"
group: "Getting Started"
order: 5
---

Once you have got inuitcss into your project using one of the [methods outlined
before](/docs/), there are a handful of things we need to do
before we’re ready to go.

Firstly, we need to identify any files whose name contain the word `example`.
These files are demo and/or scaffolding files that inuitcss requires, but that
you are encouraged to create and define yourself. These files are:

```
example.main.scss
settings/_example.settings.config.scss
settings/_example.settings.global.scss
components/_example.components.buttons.scss
```

Here’s what we need to do with them:

### [`example.main.scss`](https://github.com/inuitcss/inuitcss/blob/master/example.main.scss)

This is your main, or _manifest_, file. This is the backbone of any inuitcss
project, and it is responsible for `@import`ing all other files. This is the
file that we compile out into a corresponding CSS file.

You need to copy this file from the directory that your package manager
installed it into, and move it to the root of your `css/` directory. Once there,
rename it `main.scss`.

Next, you’ll need to update all of the `@import`s in that file to point at the
new locations of each partial (that will depend on how your project is set up).

Once you’ve done this, you should be able to run the following command on that
file and get a compiled stylesheet without any errors:

```
path/to/css/$ sass main.scss:main.css
```

**N.B.** If you downloaded inuitcss, you do not need to move this file; you
can simply rename it.

### [`_example.settings.config.scss`](https://github.com/inuitcss/inuitcss/blob/master/settings/_example.settings.config.scss)

This is a configuration file that inuitcss uses to handle the state, location,
or environment of your project. This handles very high-level settings that don’t
necessarily affect the CSS itself, but can be used to manipulate things
depending on where you are running things (e.g. turning a debugging mode on, or
telling your CI sever that you’re compiling for production).

Copy this file into your own `css/settings/` directory and rename it
`_settings.config.scss`.

**N.B.** If you downloaded inuitcss, you do not need to move this this file; you
can simply rename it.

### [`_example.settings.global.scss`](https://github.com/inuitcss/inuitcss/blob/master/settings/_example.settings.global.scss)

This is an example globals file; it contains any settings that are available to
your entire project. These variables and settings could be font families,
colours, border-radius values, etc.

Copy this file into your own `css/settings/` directory and rename it
`_settings.global.scss`. Now you can begin adding your own project-wide
settings.

**N.B.** If you downloaded inuitcss, you do not need to move this file; you
can simply rename it.

### [`_example.components.buttons.scss`](https://github.com/inuitcss/inuitcss/blob/master/components/_example.components.buttons.scss)

You don’t need to really do much with this file other than ensure you don’t let
it into your final project!

This file exists to show you how you might build components into an inuitcss
project, because components are the one thing that inuitcss purposefully refuses
to provide.

You can, if you wish, copy this file to your own `css/components/` directory and
rename it `_components.buttons.scss`. You can now use this file as the basis for
your own buttons component.
