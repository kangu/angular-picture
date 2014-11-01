# Angular Picture

Angular directive for the [Picturefill](http://scottjehl.github.io/picturefill/) responsive image polyfill.

## Installation

1. `bower install angular-picture`
2. Include `ngPicturefill` in your Angular module.

## Usage

```html
<picture picturefill>
    <!--[if IE 9]><video style="display: none;"><![endif]-->
    <!-- Preset media queries -->
    <source srcset="images/logo_4x.png" pf-media="screen-lg" />
    <source srcset="images/logo_3x.png" pf-media="screen-md"/>
    <source srcset="images/logo_2x.png" pf-media="screen-sm"/>
    <source srcset="images/logo_1x.png" pf-media="screen-xs"/>
    <!-- Custom media query -->
    <source srcset="images/logo_3x.png" pf-media="(min-width: 1000px)" />
    <!--[if IE 9]></video><![endif]-->
    <image srcset="images/logo.png" alt="Logo"/>
</picture>
```

### Preset media queries

* `screen-xs`: Extra small devices (phones, less than 768px).
	* Alias: `phone`
* `screen-sm`: Small devices (tablets, 768px and up).
	* Alias: `tablet`
* `screen-md`: Medium devices (desktops, 992px and up).
	* Alias: `desktop`
* `screen-lg`: Large devices (large desktops, 1200px and up).
	* Alias: `lg-desktop`
* `landscape`: Landscape mode.
* `portrait`: Portrait mode.
* `retina`: Retina display.
