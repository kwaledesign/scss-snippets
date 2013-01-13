# SASS and Compass Snippets for Vim's Snipmate Plugin

scss-snippets is a Vim SnipMate plugin to enable auto-completion for SCSS and much of Compass

## Installation

### Required
* Install [vim-snipmate](https://github.com/garbas/vim-snipmate)

### Install via [Pathogen](https://github.com/tpope/vim-pathogen)
    $ cd ~/.vimrc/bundle
    $ git clone https://github.com/kwaledesign/scss-snippets.git
* Reload Vim (or `:source ~/.vimrc`)

### Install via [Vundle](https://github.com/gmarik/vundle)
* Add `Bundle 'kwaledesign/scss-snippets'` to your *.vimrc*
* Reload Vim (or `:source ~/.vimrc`)
* Call `:BundleInstall` from Vim's commandline

### Manual Installation
* Put `scss.snippet` in your chosen SnipMate's `snippets/` dir
* Restart Vim
* Call `:set filetype=scss` or,
* have `filetype on` in your *.vimrc* (recommended)

## Notes
(See `scss.snippets` for the actual snippets, I've done my best to keep it well
commented).

### Sass
* Sass functions use the first three letters of the function (occ. four)

### Compass
* The majority of [Compass](http://compass-style.org/) is included, specificly: 
  * [css3 module](http://compass-style.org/reference/compass/css3/)
  * [vertical rhythm](http://compass-style.org/reference/compass/typography/vertical_rhythm/) from the typography module
  * most of the [helpers module](http://compass-style.org/reference/compass/helpers/) including sprites and grid functions.
* Included modules have snippets for variables, constants, functions, and mixins.
* Compass constants and variables are prefixed by '$', mixins are prefixed with '@', functions are unprefixed.
* Most all compass features are mapped to first letter abbreviations, for example: @dbc expands to default-background-clip
* Noted omissions: 
  * I don't find everything in the Compass framework useful. Features I don't
    use were left out. If any of these ommissions disapoint you, please file
    an issue, or even better a pull request.

## To Do
* cross reference with css spec, re-map any Compass css3 snippets using
  unneeded prefixes to unprefixed version.
* potentially expand Compass support if community demand exists

## License:
Just as the original snipMate pluginall the snippets are licensed under the
terms of the MIT license.
