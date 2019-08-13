# Sphinx Test Locale Override

Test project to debug problem I have overriding certain Sphinx translations.

I read [1] as it should be possible to add a file ``locale/<language>/LC_MESSAGES/sphinx.mo`` to the source dir (same dir as the ``Makefile``) and through that change translations or add additional translation to <language>. 

When I add ``locale/da/LC_MESSAGES/sphinx.po``, with updated entries for ``Fig. %s`` and ``Listing %s``, a ``locale/da/LC_MESSAGES/sphinx.mo`` is created (because of ``gettext_auto_build = True``), but the translations are note used. The translations from the official ``da`` translation [2] is used.

[1] http://www.sphinx-doc.org/en/master/usage/configuration.html#confval-locale_dirs
[2] https://github.com/sphinx-doc/sphinx/blob/master/sphinx/locale/da/LC_MESSAGES/sphinx.po
