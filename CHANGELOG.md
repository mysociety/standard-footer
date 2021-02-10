# Standard mySociety Footer Changelog

## v1.0.8

* New `$mysoc-footer-horizontal-gutter` variable, to control the horizontal
  space between list items / organisation logos. Previously hard-coded at 1em,
  which would cause overflow issues on sites that had less than 1em (16px) of
  padding either side of their containers on narrow screens (eg: WriteToThem,
  which has a 15px container padding).

## v1.0.7

* Update legal text to use mySociety and SocietyWorks, rather than UKCOD and
  mySociety Ltd.

## v1.0.6

* Remove all 2x PNGs as they are not needed.

## v1.0.5

* Fix Sass bug which was causing browsers with SVG image background support to
  ignore the SVG rules and instead display the @2x PNG backgrounds.

## v1.0.4

* Stop empty columns (using the styles in mysoc-footer-example-grid.scss) from
  vertically collapsing, by giving columns a min-height.

## v1.0.3

* Legal text in the example footer HTML no longer includes the registered
  company numbers, and instead links to mysociety.org where full company
  details and contact details can be found.
* Added contribution guidelines to the repo, documenting how and when to issue
  new versions/releases of the footer.

## v1.0.2

* List items inside `.mysoc-footer__links` now have better vertical spacing.
  Especially useful for clearly differentiating between list items that wrap
  onto multiple lines.

## v1.0.1

* `box-sizing: border-box` is now correctly set for the `.mysoc-footer` and all
  of its children.
* Links to mysociety.org in the HTML template now start with www to avoid an
  unnecessary redirect. (Thanks @dracos!)

## v1.0.0

* The hard-coded slashes in image urls have been removed, meaning we avoid
  double slashes when `$mysoc-footer-image-path` correctly ends in a slash.
* `$mysoc-footer-border-top-color` has been replaced with a more general
  `$mysoc-footer-border-top`, allowing you to define a custom border-width or
  border-style in addition to the border-color, without having to write your
  own override rule. See the demo for an example of how this new variable
  should be used.
* The top of `.mysoc-footer__links` will now always match the top of
  `.mysoc-footer__site-description`, regardless of how the parent site defines
  line-height for headings.
* Styling for the example partner logo (Horse) was moved from the core styles
  into the demo styles, since it’s only an example.

## v0.1.0

* Added version number to project!
* Demo site included in `/demo`.
