=============================================================================
django-variable-admin -- Administration interface styling using CSS variables
=============================================================================

This project allows changing the colors used in Django's administration
panel using CSS variables. It is an import of the code in
https://github.com/django/django/pull/13435 into a standalone repository
with the aims of allowing testing and maybe, in the future, allowing to
use CSS variables when not using the latest and best Django version.


Usage
=====

``python -m pip install django-variable-admin`` inside your project and
insert ``variable_admin`` **before** ``django.contrib.admin`` into
``INSTALLED_APPS``.

.. code-block:: python

    INSTALLED_APPS = [
        ...
        "variable_admin",
        "django.contrib.admin",
        ...
    ]

``./manage.py collectstatic`` now complains about duplicates with the
same destination path. That's to be expected.


Compatibility
=============

Assuming that the pull request
https://github.com/django/django/pull/13435 lands in Django 3.2 this package
is only useful for Django <= 3.1.x.
