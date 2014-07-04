
Introduction to portfolio

portfolio boasts a clean HTML5 structure with extensible CSS classes and ID's for unlimited
theming possibilities as well as a top-down load order for improved SEO. It is fully
responsive out-of-the-box and provides an adaptive, elegant, SASS based grid system (Bourbon Neat).

portfolio's goal is to provide themers the building blocks needed to get their designs up and
running quickly and simply.

portfolio is perfect if you want a simple, smart, and flexible theme starter.

Less code spam, more ham.

__________________________________________________________________________________________

Installation

- portfolio utilizes SASS for adaptive grids and layouts and general structure of the site.
  It's recommended to use SASS for building out your theme. You are required to download
  the following Ruby Gems and plugins:

  - SASS (http://sass-lang.com/)
  - Bourbon (http://bourbon.io/)
  - Boubon Neat (http://neat.bourbon.io/)

- portfolio is meant to be YOUR theme. To change the name of the theme from 'portfolio' to another name like 'mytheme',
follow these steps (to do BEFORE enabling the theme) :

    - rename the theme folder to 'mytheme'
    - rename portfolio.info to mytheme.info
    - Edit portfolio.info and change the name, description, project (can be deleted), replace all other instances of "portfolio" ie. [portfolio_tabs] would become [mytheme_tabs]
    - In template.php change each iteration of 'portfolio' to 'mytheme'
    - In theme-settings.php change each iteration of 'portfolio' to 'mytheme'

__________________________________________________________________________________________

What are the files for ?
------------------------

- portfolio.info                => provide informations about the theme, like regions, css, settings, js ...
- block-system-main.tpl.php => template to edit the content
- block.tpl.php             => template to edit the blocks
- comment.tpl.php           => template to edit the comments
- node.tpl.php              => template to edit the nodes (in content)
- page.tpl.php              => template to edit the page
- template.php              => used to modify drupal's default behavior before outputting HTML through
                               the theme
- theme-settings            => used to create additional settings in the theme settings page

In /SASS
-------

- default.sass  => define default classes, browser resets and admin styles (compiles to css/default.css)
- ie8.sass      => used to debug IE8 (compiles to css/ie8.css)
- ie9.sass      => used to debug IE9 (compiles to css/ie9.css)
- layout.sass   => define the layout of the theme (compiles to css/layout.css)
- print.sass    => define the way the theme look like when printed (compiles to css/print.css)
- style.sass    => contains some default font styles. that's where you can add custom css (compiles to css/style.css)
- tabs.sass     => styles for the admin tabs (from ZEN)

__________________________________________________________________________________________

Changing the Layout

The layout used in portfolio is fairly similar to the Holy Grail method. It has been tested on
all major browser including IE (5>10), Opera, Firefox, Safari, Chrome ...
The purpose of this method is to have a minimal markup for an ideal display.
For accessibility and search engine optimization, the best order to display a page is ]
the following :

    1. header
    2. content
    3. sidebars
    4. footer

This is how the page template is buit in portfolio, and it works in fluid and fixed layout.
Refers to the notes in layout.css to see how to modify the layout.

__________________________________________________________________________________________

UPDATING portfolio

Once you start using portfolio, you will massively change it until a point where it has nothing
to do with portfolio anymore. Unlike ZEN, portfolio is not intended to be use as a base theme for a
sub-theme (even though it is possible to do so). Because of this, it is not necessary to
update your theme when a new version of portfolio comes out. Always see portfolio as a STARTER, and
as soon as you start using it, it is not portfolio anymore, but your own theme.

If you didn't rename your theme, but you don't want to be notified when portfolio has a new version
by the update module, simply delete "project = "portfolio" in portfolio.info

__________________________________________________________________________________________

Thanks for using portfolio, and remember to use the issue queue in drupal.org for any question
or bug report:

http://drupal.org/project/issues/portfolio

Current maintainers:
* Steve Krueger (SteveK) -http://drupal.org/user/111656 (http://thejibe.com)
* Niall Morgan (lil.destro) -https://drupal.org/user/597808 (http://thejibe.com)