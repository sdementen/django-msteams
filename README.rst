=============================
Django MS Teams
=============================

.. image:: https://badge.fury.io/py/django-msteams.svg
    :target: https://badge.fury.io/py/django-msteams

.. image:: https://travis-ci.org/sdementen/django-msteams.svg?branch=master
    :target: https://travis-ci.org/sdementen/django-msteams

.. image:: https://codecov.io/gh/sdementen/django-msteams/branch/master/graph/badge.svg
    :target: https://codecov.io/gh/sdementen/django-msteams

Django app to send messages to a MS Teams channel

Documentation
-------------

The full documentation is at https://django-msteams.readthedocs.io.

Quickstart
----------

Install Django MS Teams::

    pip install django-msteams

Add it to your `INSTALLED_APPS`:

.. code-block:: python

    INSTALLED_APPS = (
        ...
        'django_msteams.apps.DjangoMSTeamsConfig',
        ...
    )

Add Django MS Teams's URL patterns:

.. code-block:: python

    from django_msteams import urls as django_msteams_urls


    urlpatterns = [
        ...
        url(r'^', include(django_msteams_urls)),
        ...
    ]

Features
--------

* TODO

Running Tests
-------------

Does the code actually work?

::

    source <YOURVIRTUALENV>/bin/activate
    (myenv) $ pip install tox
    (myenv) $ tox

Credits
-------

Tools used in rendering this package:

*  Cookiecutter_
*  `cookiecutter-djangopackage`_

.. _Cookiecutter: https://github.com/audreyr/cookiecutter
.. _`cookiecutter-djangopackage`: https://github.com/pydanny/cookiecutter-djangopackage
