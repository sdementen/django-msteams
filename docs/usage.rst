=====
Usage
=====

To use Django MS Teams in a project, add it to your `INSTALLED_APPS`:

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
