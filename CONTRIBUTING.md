# Contributing to the standard footer

Once you’ve added new commits, you’ll want to properly release a new version of
the footer.

We use Semantic Versioning for the standard mySociety footer. A clear
versioning system helps make it obvious which version of the footer each site
is using.

Daniel at Optimizely gave some good examples of
[how to apply SemVer to CSS modules](https://medium.com/design-optimizely/how-to-version-your-ui-library-1c7a1b7ee23a#.8dvyzmvek).

Generally:

* If you’ve made *minor, non-breaking changes* or *bug fixes*, then you will
  want to release a patch, ie: increment the third part of the version number,
  eg: 1.0.4 => 1.0.5
* If you’ve made *larger, but still backwards-compatible* changes, like adding
  new optional components or new backwards-compatible variables, then you will
  want to release a minor version, ie: increment the second part of the version
  number, eg: 1.0.4 => 1.1.0
* If you’ve made *breaking changes*, like removing styles or mixins that
  individual implementations of the footer might rely on, then you will want to
  release a major version, ie: increment the first part of the version number,
  eg: 1.0.4 => 2.0.0

Once you’ve decided what version number to increment to, do the following:

1. Update the version number at the top of `./mysoc-footer.scss`
2. Add a section to `./CHANGELOG.md`, explaining the changes in this version.

And finally (swapping `1.x.x` for the version number you’ve chosen):

    git commit -m "Changelog for version 1.x.x"
    git tag -a v1.x.x -m "Version 1.x.x of the Standard mySociety Footer."
    git push origin HEAD --tags

Note how the git tags, specifically, are named with a "v" preceding the version
number, like `v1.0.4`.
