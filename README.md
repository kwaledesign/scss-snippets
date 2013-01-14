# SASS and Compass Snippets for Vim's Snipmate Plugin

scss-snippets is a Vim SnipMate plugin to enable auto-completion for SCSS and much of Compass. It also includes a revised version of [honza's]()
  [css.snippets](https://github.com/honza/snipmate-snippets/blob/master/snippets/css.snippets) to facilitate granular control over snippet collisions and to closely integrate with Compass allowing for quicker updates as browsers drop the prefixed versions of CSS properties.

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
See `scss.snippets` for the actual snippets.

### Sass
* Most SassScript functions use the first three letters of the function.

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

### CSS
* The majority of [honza's]()
  [css.snippets](https://github.com/honza/snipmate-snippets/blob/master/snippets/css.snippets)
  are included, along with the following modifications:
  * All prefixed css properties were removed in favor of the above Compass CSS3
    Module snippets
  * Also, the ability to tab out of the current property into a new line was
    added to each css snippet. This functionality is consistient with both the
    Sass and Compass snippets.

## To Do
* Remove Compass CSS3 prefixed snippets and remap to the unprefixed CSS3
  versions as needed.
* Potentially expand Compass support if community demand exists

## License:
scss-snippets is licensed under the terms of the MIT license.
