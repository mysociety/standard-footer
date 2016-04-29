# Standard mySociety footer

The reference implementation of the standard mySociety footer, for use across all of the sites we operate.

![Screenshot of light theme footer](/screenshot-light.jpg?raw=true)

![Screenshot of dark theme footer](/screenshot-dark.jpg?raw=true)

## Preview

There is a demonstration of the footer, and how it can be customised, in the `/demo` directory.

    gem install jekyll
    cd demo
    jekyll serve

## How to implement the footer in your project

Copy `/mysoc-footer.scss` to your project (perhaps in a `/vendor` directory, or somewhere self-documenting) and import it into your Sass pipeline just like any other 3rd-party Sass module.

Then, add markup to your project’s HTML templates, that satisfies the standard mySociety footer’s requirements. See `/demo/_includes/footer.html` for an example, and `/demo/_sass/style.scss` for documentation on how to override the footer’s default behaviours.
