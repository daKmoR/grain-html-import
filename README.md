[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg)](https://www.webcomponents.org/element/daKmoR/grain-html-import)
[![Polymer Version](https://img.shields.io/badge/polymer-v2-blue.svg)](https://www.polymer-project.org)

# \<grain-html-import\>

Only import Html if certain conditions are met.

## Problem
```html
<link rel="import" href="path/to/my-bundle.html">
<link rel="import" href="path/to/my-element">
```

If `my-bundle.html` contains `my-element` it will be imported again as rel="import" only checks for the href path.
In order to provide some additional condition before importing you can use `grain-html-import`.

## Installation

```sh
$ bower install --save daKmoR/grain-html-import
```

## Getting Started

Import the package.

```html
<link rel="import" href="/bower_components/grain-html-import/grain-html-import.html">
```

Use the import just as you would rel="import" but provide some conditions.

```html
<grain-html-import href="path/to/my-element.html" if-tag-not-available="my-element"></grain-html-import>
```

*For more information, see the API documentation.*

## Working on the Element

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed.
* View the Element via `polymer serve`
* Run tests via `polymer test`
