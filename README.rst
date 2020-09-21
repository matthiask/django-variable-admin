=============================================================================
django-variable-admin -- Administration interface styling using CSS variables
=============================================================================

Usage
=====

Use this to insert a script tag via ``forms.Media`` containing additional
attributes (such as ``id`` and ``data-*`` for CSP-compatible data
injection.):

.. code-block:: python

    INSTALLED_APPS = [
        ...
        "variable_admin",
        "django.contrib.admin",
        ...
    ]


Compatibility
=============

Assuming that the pull request
https://github.com/django/django/pull/13435 lands in Django 3.2 this package
is only useful for Django <= 3.1.x.
