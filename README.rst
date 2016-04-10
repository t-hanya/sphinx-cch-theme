====================
Sphinx CCH Theme
====================

Original Sphinx Theme

Requirements
=============

- Python
- Sphinx

Apply theme to your document
================================

Please edit ``conf.py`` in your sphinx project directory::

   html_theme = 'sphinx_cch_theme'
   html_theme_path = ["/path/to/dir"]   # contains sphinx_cch_theme

Build demo site
===================

Build demo site::

   $ pip install -U sphinx  # if necessary
   $ git clone <this repository>
   $ cd sphinx-cch-theme/demo
   $ make html

And please open `./_build/html/index.html`

License
=========

MIT License


