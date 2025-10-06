# Pattern Template 7-1 version with Split Media

An extraordinarily neat architecture that any Web Designer can understand at a glance. Structure with the help of SASS and media queries.

## SASS

``` txt
sass/
|
|– abstracts/
|   |– _mixins.sass
|   |– _variables.sass
|– base/
|   |– _base.sass
|   |– _fonts.sass
|   |– _helpers.sass
|   |– _typography.sass
|– mobile/
|   |– layout/
|   |   |– _footer.sass
|   |   |– _header.sass
|   |– components/
|   |   |– _alert.sass
|   |   |– _button.sass
|   |   |– ...
|   |– pages/
|   |   |– _home.sass
|   |   |– _contact.sass
|   |   |– ...
|– desktop/
|   |– layout/
|   |   |– _footer.sass
|   |   |– _header.sass
|   |– components/
|   |   |– _alert.sass
|   |   |– _button.sass
|   |   |– ...
|   |– pages/
|   |   |– _home.sass
|   |   |– _contact.sass
|   |   |– ...
|– themes/
|   |– _dark.sass
|   |– _light.sass
|– vendors/
|   |– _normalize.sass
|   |– _owl-carousel.sass
|   ...
`– mobile.sass
`– desktop.sass
`- (any other size we need)
