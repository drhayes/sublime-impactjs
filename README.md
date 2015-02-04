# ImpactJS for Sublime Text 2

A collection of snippets and shortcuts for doing ImpactJS development in Sublime
Text 2.

*Issues and pull requests welcome!* I don't use Sublime these days so I'm less
aware of the little daily pains that using this package can cause. Please let
me know if there's something missing that you want and we'll work to get it
in here.

## Install

Please use [Package Control][packagecontrol] to install the ImpactJS plugin for
Sublime Text 2. Everything else would just be terrible.

  [packagecontrol]: https://packagecontrol.io/

## Usage

This package is careful to not steal your JS syntax away from you. To use this
package in Sublime you must switch the syntax of your current file from
"JavaScript" to "ImpactJS".

By default, you can press <kbd>CTRL</kbd> - <kbd>SHIFT</kbd> - <kbd>P</kbd> to
pull up the syntax chooser.

## Snippets

I really love <kbd>TAB</kbd> completion snippets. Once your syntax is switched
(see above), you can type the shortcuts below, hit <kbd>TAB</kbd>, and the
snippet should expand in place.

See the [Sublime documentation for "Snippets" for more info][snippets].

  [snippets]: http://docs.sublimetext.info/en/latest/extensibility/snippets.html

### `igm`

Define an Impact module. By default, the snippet defines the module with a
`'use strict';` expression to force JS into [strict mode][strict]. Trust me,
you want this. But it *does* mean that your definitions probably have to be
declared with a `window` in front of them. For example:

     window.EntityPlayer = ig.Entity.extend({});

### `ige`

Define an Impact entity. As above, the module will be in [strict mode][strict].

  [strict]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Strict_mode

## Completions

This package knows about certain properties in Impact and will help you complete
them by pressing <kbd>CTRL</kbd> - <kbd>SPACE</kbd>.

See the [Sublime docs about "Completions" for more info][completions].

  [completions]: http://docs.sublimetext.info/en/latest/extensibility/completions.html

### Entity

All the [Entity][entity] properties and methods.

  [entity]: http://impactjs.com/documentation/class-reference/entity

### Keys

All the [mouse and keyboard names][keys].

  [keys]: http://impactjs.com/documentation/class-reference/input#mouse-and-keyboard-button-names
