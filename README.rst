=============================================================================
django-variable-admin -- Administration interface styling using CSS variables
=============================================================================

This project allows changing the colors used in Django's administration
panel using CSS variables. It only contains a copy of the CSS files
which will be a part of the upcoming Django 3.2 release. The project is
mainly intended for those who want to get their hands on the new theming
and dark mode support a little bit earlier.

Also, if things do not look right *please* report those issues to the
Django project (maybe while adding me to the Cc:) so that they can be
fixed there.


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
