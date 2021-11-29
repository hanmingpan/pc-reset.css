# minirem.css

![GitHub](https://img.shields.io/github/license/mashape/apistatus.svg)

A mobile layout css with rem

- no javascript
- prefer to use unit `vw`

# Install
    npm i minirem.css --save

# Usage
- based on 750px design draft
- 1rem = 100px

## Module
    import 'minirem.css'

## Browser
    <link rel="stylesheet" href="minirem.css">

## CDN
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/minirem.css">

# Example

## css
    .main {
        width: 1rem; // 100px
    }

## sass
    // variable.scss
    $baseFontSize:100;

    @function px2rem($px){
        @return $px / $baseFontSize * 1rem;
    }

    // index.scss
    @import "variable";

    .main {
        width: px2rem(100);
    }
