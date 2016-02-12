# Common styling units for EA-branded data.gov.uk web sites

This site contains some re-usable elements that can provide some
commonality between our various EA-branded data.gov.uk web sites.
In particular, a common top navigation bar and common footer.
Other common elements may be added in future.

## Assets provided

* `sass/_ea-brand.scss`
  Common brand elements as re-usable SASS variables, including colour palette.

* `sass/_page-top-bar.scss`
  Styling for a common page top bar, including logo as SVG (with PNG fallback for older browsers), proposition title and menu

* `sass/_page-footer.scss`
  Styling for a common page footer, including support links and linked data
  logo.

* `html/page-top-bar.hbs`
  Example markup for page top bar as a Handlebars template (actually very close to HTML)

* `html/page-footer.hbs`
  Example markup for page footer as a Handlebars template (actually very close to HTML)

* `images`
  Contains common brand images as `.svg` and `.png` files

## Generating the stylesheets

In a Sass-based project, the `.scss` files can be imported as-is. For projects
using plain CSS, use `css/ea-common.css`. This file is auto-generated from the Sass sources, but requires Bootstrap to be installed via bower first:

    bower install
    sass -I bower_components sass/ea-common.scss > css/ea-common.css
