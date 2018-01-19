zero config `<zero-md>`
======================

> Share rendered markdown files without upkeep. Fully-encapsulated fork of [`<zero-md>`][zero-md].


## Install
```sh
$ curl -O https://raw.githubusercontent.com/knksmith57/zero-config-zero-md/master/docs/index.html
```


## Usage
`./README.md` is loaded by default; use `?file=<path>` to specify a different markdown file:

```sh
## zeit/serve
$ npx serve -p 8080

## ./README.md (default)
$ open http://localhost:8080

## explicitly load ./README.md
$ open http://localhost:8080?file=README.md

## ./CONTRIBUTING.md
$ open http://localhost:8080?file=CONTRIBUTING.md

## _this_ README.md
$ open http://localhost:8080?file=https://raw.githubusercontent.com/knksmith57/zero-config-zero-md/master/README.md
```


## Why?
I needed a cheap way to share rendered markdown files without upkeep. [`zero-md`][zero-md] _almost_ did it.

[@zerodevx] glued a bunch of really great tools and ideas together into a clean, composable webcomponent with
_really good [documentation][zero-md-docs]_!

Unfortunately, the user is required to:
* host a handful of static assets _or_ rely on third-party CDNs
* modify `index.html` to render a new / different markdown file

This is really not a big deal. I'm just super lazy, so here's a single `index.html` file that uses a `?file=` query param to do all that ^^ instead.


## License
Powered by cool stuff from cool people:
* [`zero-md`][zero-md] by [@zerodevx]
* [`marked`][marked] by [@chjj]
* [GFM theme][gfm-theme] by [@sindresorhus]
* [GHColors theme][ghc-theme] by [@aviaryan]
* [h5bp]
* [Polymer]
* [PrismJS]

Anything that's left is yours under [MIT].


## ♥︎
Assembled with `<3` by [@knksmith57]


[ghc-theme]: https://github.com/PrismJS/prism-themes/blob/master/themes/prism-ghcolors.css
[gfm-theme]: https://github.com/sindresorhus/github-markdown-css
[h5bp]: https://github.com/h5bp/html5-boilerplate
[marked]: https://github.com/chjj/marked
[MIT]: https://choosealicense.com/licenses/mit/
[Polymer]: https://github.com/Polymer/polymer
[PrismJS]: https://github.com/PrismJS/prism
[zero-md]: https://github.com/zerodevx/zero-md
[zero-md-docs]: https://zerodevx.github.io/zero-md/

[@aviaryan]: https://github.com/aviaryan
[@chjj]: https://github.com/chjj
[@knksmith57]: https://twitter.com/knksmith57
[@sindresorhus]: https://github.com/sindresorhus
[@zerodevx]: https://github.com/zerodevx

