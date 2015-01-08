lintel-contrib-badges
=====================

> Badges for lintel.

[![npm](https://img.shields.io/npm/v/lintel-contrib-badges.svg)](https://www.npmjs.com/package/lintel-contrib-badges)
[![Bower](https://img.shields.io/bower/v/lintel-contrib-badges.svg)](https://github.com/lintelio/lintel-contrib-badges)


## Getting Started
This module requires Lintel.

If you haven't used [Lintel](http://lintel.io/) before, be sure to check out the [Getting Started](http://lintel.io/getting-started) guide, as it explains how to install and use this module. Once you're familiar with that process, you may install this module with this command:

```shell
bower install lintel-contrib-badges --save
```

Once the module has been installed, you will have to load it in your main SASS file:

```scss
@import "bower_components/lintel-contrib-badges/sass/badges.scss"
```

You can use [wiredep](https://github.com/taptapship/wiredep) or [grunt-wiredep](https://github.com/stephenplusplus/grunt-wiredep) to automatically inject files in your build process.


## Variables
Check the vars file in the `sass` folder to see the full list of variables you can customize.

#### $badge-padding-y
Default value: `4px`  

Badge padding-top and padding-bottom.

#### $badge-padding-y
Default value: `4px`  

Badge padding-top and padding-bottom.

#### $badge-padding-x
Default value: `8px`  

Badge padding-left and padding-right.

#### $badge-border-radius
Default value: `$border-radius-sm`  

Badge border-radius.


## Mixins
Check the mixins file in the `sass` folder to see how you can extend this module.

#### make-badge($bg, [$border, $text, $bg-inverse, $border-inverse, $text-inverse])
Sets the background, border, and text color of a badge. Only include `$*-inverse` parameters if `$badge-include-inverse` is `true`.

```scss
.badge-primary {
  @include make-badge(
    $bg: $badge-primary, 
    $bg-inverse: $badge-primary-bg,
    $border-inverse: $badge-primary-border, 
    $text-inverse: $badge-primary-text
  );
}
```


## Examples

#### Base
```html
<span class="badge">Default</span>
```

#### Primary Badge
```html
<span class="badge">Primary</span>
```

#### Round Badge
```html
<h1>CSS makes the world go <span class="badge badge-round">round</span></h1>
```

#### Inside Headings
```html
<h1>This is a big, bad <span class="badge">badge</span></h1>
```


## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).


## License
Copyright (c) 2015 Marius Craciunoiu. Licensed under the MIT license.
