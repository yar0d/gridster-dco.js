Gridster.js
===========

[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/ducksboard/gridster.js/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

Gridster is a jQuery plugin that makes building intuitive draggable
layouts from elements spanning multiple columns. You can even
dynamically add and remove elements from the grid.

More at [http://gridster.net/](http://gridster.net/).

[Releases](https://github.com/ducksboard/gridster.js/releases)

[CHANGELOG](https://github.com/ducksboard/gridster.js/blob/master/CHANGELOG.md)

Gridster is maintained by Ducksboard occasionally but not actively.
@dustmoo and @pushmatrix have also write permissions as Gridster maintainers
they are. Thank you guys!

## This Fork

This fork to introduce a scale value, as in CSS 3 scale attribute. I use it to do CSS scaling and keep mouse move at the right scale. You must provide scale in both resize and draggable options.

Example:
```
$('#tiles').gridster({
    namespace: '#tiles',
    widget_margins: [4, 4],
    widget_base_dimensions: [100, 100],
    avoid_overlapped_widgets: true,
    min_cols: config.columns,
    extra_cols: 2,
    extra_rows: 2,
    autogrow_cols: true,
    resize: {
        scale: 0.6,
        enabled: true,
        helper: 'clone',
        handle_append_to: '.header.widget-title:visible'
    },
    draggable: {
        scale: 0.6
    }
});

gridster = $('#tiles').gridster().data('gridster');
```
## Other Forks

Mr @dustmoo (maintainer of Gridster) has his own fork of gridster.js
with some new interesting features like widget-swapping and static widgets.

Can be found here: [dustmoo/gridster.js](https://github.com/dustmoo/gridster.js)

@dustmoo is working in his spare time to merge all these changes into
ducksboard/gridster.js

If anyone would like to help @dustmoo improve his fork and reconcile
it with the main library he would be happy for the help.


## Contributing to this project

Anyone and everyone is welcome to contribute. Please take a moment to review the guidelines for contributing.

* [Bug reports](CONTRIBUTING.md#bugs)
* [Feature requests](CONTRIBUTING.md#features)
* [Pull requests](CONTRIBUTING.md#pull-requests)


## License

Distributed under the MIT license.

## Whodunit

Gridster is built by [Ducksboard](http://ducksboard.com/) with the help of all
these [wonderful people](https://github.com/ducksboard/gridster.js/graphs/contributors).
