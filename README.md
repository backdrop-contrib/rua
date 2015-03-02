Remove Uppercase Accents (rua)
==============================

Automatically removes accented characters (currently greek) from elements having
their text content uppercase transformed through CSS.

This project is now called 'rua'.
It used to be called 'remove_upcase_accents'.
On Drupalcon Prague I discussed with people about it and we agreed that
it should either something short or 'remove_upPERcase_accents'.
We chose the short name :)

Installation
------------

- Install this module using the official Backdrop CMS instructions at
  https://backdropcms.org/guide/modules

Usage
-----

The script operates automatically on the document ready event, by selecting all
the elements having their text content uppercase transformed through CSS, and by
replacing the accented characters in them by their respective non-accented.

The selection is based on the effective CSS rules defining the uppercase text
transformation, ie the following style rule:

  h1 { text-transform: uppercase; }

or

  .title { font-variant: small-caps; }

Currently the script transforms only greek text, but it can be easiy extended
to support other languages.


License
-------

This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.


Current Maintainers
-------------------

- Bill Seremetis (https://github.com/bserem/)


Credits
-------

This module was originally written for Drupal by Bill Seremetis
(https://drupal.org/u/bserem), based on Thanasis Doumas 
remove-upcase-accents project
(https://github.com/tdoumas/jquery-remove-upcase-accents).
