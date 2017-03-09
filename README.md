# Changelog

## 9.3.2017

New custom events (jQuery)
- `softpage:opened`: triggered when softpage has been opened
- `softpage:closed`: triggered when softpage has been closed
- `form-modal:opened`: triggered when form-modal has been opened
- `form-modal:closed`: triggered when form-modal has been closed

How to listen to these events:
```JavaScript
$(window).on('softpage:opened form-modal:opened', function() {
    // do something
});
```

## 7.3.2017

- `tingle.js` close button is now working properly when multiple tingle instances are present.
- In progress: Static files of default social icons defined in `allink-core` will soon be moved to `allink-core-static`

## 6.3.2017

- All `input` fields with the `maxlength` attribute are now forcefully limitted via the `initFormModifications` function.

## 1.3.2017

New variables available:

### overlay

```SCSS
$overlay-background-color-sm-max:          #000;
$overlay-background-opacity-sm-max:        0.5;
```

### swiper

```SCSS
$swiper-default-pagination-hidden-sm-max:       true;
```

## 25.1.2017

New variables available:

```SCSS
/* * * * * * * * * * * * * * * * * * * * * * * * * * * * * *

=Alerts

*/

$alert-border-width:            1px;
$alert-border-style:            solid;
$alert-border-color:            transparent;
$alert-padding:                 1em 1em 1em 3em; // Important: Leave some space for the icon!
$alert-icon-position-left:      1em;

$alert-variations: (
    'success': (
        'icon':                 '\e206',
        'icon-color':           $brand-success-dark,
        'border-color':         $brand-success,
        'bg':                   $brand-success-light,
        'color':                $brand-success-dark,
    ),
    'danger': (
        'icon':                 '\e000',
        'icon-color':           $brand-danger-dark,
        'border-color':         $brand-danger,
        'bg':                   $brand-danger-light,
        'color':                $brand-danger-dark,
    ),
    'warning': (
        'icon':                 '\e002',
        'icon-color':           $brand-warning-dark,
        'border-color':         $brand-warning,
        'bg':                   $brand-warning-light,
        'color':                $brand-warning-dark,
    ),
    'info': (
        'icon':                 '\e2a2',
        'icon-color':           $brand-info-dark,
        'border-color':         $brand-info,
        'bg':                   $brand-info-light,
        'color':                $brand-info-dark,
    ),
);
```
