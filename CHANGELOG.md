# Standard mySociety Footer Changelog

## v1.0.1

* `box-sizing: border-box` is now correctly set for the `.mysoc-footer` and all of its children.
* Links to mysociety.org in the HTML template now start with www to avoid an unnecessary redirect. (Thanks @dracos!)

## v1.0.0

* The hard-coded slashes in image urls have been removed, meaning we avoid double slashes when `$mysoc-footer-image-path` correctly ends in a slash.
* `$mysoc-footer-border-top-color` has been replaced with a more general `$mysoc-footer-border-top`, allowing you to define a custom border-width or border-style in addition to the border-color, without having to write your own override rule. See the demo for an example of how this new variable should be used.
* The top of `.mysoc-footer__links` will now always match the top of `.mysoc-footer__site-description`, regardless of how the parent site defines line-height for headings.
* Styling for the example partner logo (Horse) was moved from the core styles into the demo styles, since it’s only an example.

## v0.1.0

* Added version number to project!
* Demo site included in `/demo`.
