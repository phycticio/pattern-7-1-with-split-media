Here is the revised `README.md` using **pnpm** instead of **yarn** for the installation and compilation steps.

````markdown
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
````

## HTML

```html

<!doctype html>
<html lang="en">
    <head>
        <meta charset="UTF-8"/>
        <title>Split media</title>
        <meta name="viewport" content="width=device-width, initial-scale=1.0, shrink-to-fit=no">
        <link href="css/mobile.css" rel="stylesheet" media="all and (max-width: 600px)">
        <link href="css/desktop.css" rel="stylesheet" media="all and (min-width: 600px)">
        </head>
    <body>
        <h1>Gravida arcu ac tortor.</h1>
    </body>
</html>
```

-----

# Compile SASS.

## Install

```bash
pnpm add -g node-sass
```

## Run

```bash
node-sass --output-style compressed sass/mobile.sass css/mobile.css
node-sass --output-style compressed sass/desktop.sass css/desktop.css
```
