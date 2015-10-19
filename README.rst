.. -*- coding: utf-8; -*-

=====================
Pelican Pure Template
=====================

Overview
========

This is a pelican theme using `Pure.css <http://purecss.io/>`_.
The theme is designed for Japanese blog.

This theme is **NOT FULLY TESTED**.
Bug fix pull requests are welcome.

Requires
========

* Pelican >= 3.6

  * Install the tag cloud plugin if you want to display tag cloud on a sidebar.

TODO
====

* Sidebar is under development.

How to Install?
===============

Clone this repository:

.. code-block:: bash

   % git clone https://github.com/pman0214/pelican-pure.git

Configure your :code:`pelicanconf.py` as:

.. code-block:: python

   % THEME = /path/to/pelican-pure

Usage
=====

Basic
-----

This theme supports the following standard Pelican settings:

* Feeds

  * :code:`FEED_ALL_ATOM`
  * :code:`FEED_ALL_RSS`

* Template settings

  * :code:`DISPLAY_PAGES_ON_MENU`
  * :code:`DISPLAY_CATEGORIES_ON_MENU`
  * :code:`MENUITEMS`

Extra
-----

Fontawesome
~~~~~~~~~~~

If you want to use `font awesome <https://fortawesome.github.io/Font-Awesome/>`_ fonts, define :code:`USE_FONT_AWESOME` in your :code:`pelicanconf.py`.

Article Info
~~~~~~~~~~~~

Set :code:`SHOW_ARTICLE_AUTHOR` to :code:`True` to show the author on articles and static pages.

Code Highlighting
~~~~~~~~~~~~~~~~~

This theme uses `Pygments <http://pygments.org/>`_  to highlight code blocks.
Set a value below to :code:`PYGMENTS_STYLE` to change highlighting style:

* autumn
* borland
* bw
* colorful
* default
* emacs
* friendly
* fruity
* github
* manni
* monokai
* murphy
* native
* pastie
* perldoc
* tango
* trac
* vim
* vs
* zenburn

Default style is :code:`github`.

Custom Site Logo
~~~~~~~~~~~~~~~~

Set :code:`SITELOGO` to specify a site logo image:

.. code-block:: python

   SITELOGO = 'images/logo.png'

Favicon
~~~~~~~

Set :code:`FAVICON` to specify a site favicon:

.. code-block:: python

   FAVICON = 'images/favicon.ico'

About Me on Sidebar
~~~~~~~~~~~~~~~~~~~

You can include `About me' block on sidebar instead of an `About me' page.
Set :code:`ABOUT_ME` to describe yourself:

.. code-block:: python

   ABOUT_ME = 'Hi!  I'm Shigemi, a researcher in Japan.'

You can use your avatar :code:`AVATAR` variable:

.. code-block:: python

   AVATAR = 'images/myself.png'

OpenGraph
~~~~~~~~~

If you **DO NOT** want to include OpenGraph tags, set :code:`USE_OPEN_GRAPH` to :code:`False`.

By default, no OpenGraph image tag is embedded.
You can embed OpenGraph image tag by specifying image file path using :code:`OPEN_GRAPH_IMAGE`:

.. code-block:: python

   OPEN_GRAPH_IMAGE = 'images/mysite-img.png'

Facebook App ID can be embedded by using :code:`OG_FB_APP_ID`.

Copyright, License
==================

* Copyright (c) 2015, Shigemi ISHIDA
* Copyright 2013 Yahoo! Inc. All rights reserved.

This software is released under the BSD 3-clause license.
See :code:`LICENSE`.

Files listed below are retrieved from `Pure.css <http://purecss.io/>`_ and are also released under BSD license.
See :code:`LICENSE-pure.md`.

* :code:`static/css/pure-min.css`
* :code:`static/css/grids-responsive-min.css`
* :code:`static/css/grids-responsive-old-ie-min.css`
