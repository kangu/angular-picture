# Angular Picture

Angular directive for the [Picturefill](http://scottjehl.github.io/picturefill/) responsive image polyfill.

## Usage

```
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

* `screen-xs`
	* Alias: `phone`
* `screen-sm`
	* Alias: `tablet`
* `screen-md`
	* Alias: `desktop`
* `screen-lg`
	* Alias: `lg-desktop`
* `landscape`
* `portrait`
* `retina`
