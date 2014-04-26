Django APS Process
============

A reusable Django app that does nothing much.

Installation
------------

To get the latest stable release from PyPi

.. code-block:: bash

    pip install django-aps-process

To get the latest commit from GitHub

.. code-block:: bash

    pip install -e git+git://github.com/bitmazk/django-aps-process.git#egg=aps_process

TODO: Describe further installation steps (edit / remove the examples below):

Add ``aps_process`` to your ``INSTALLED_APPS``

.. code-block:: python

    INSTALLED_APPS = (
        ...,
        'aps_process',
    )

Add the ``aps_process`` URLs to your ``urls.py``

.. code-block:: python

    urlpatterns = patterns('',
        ...
        url(r'^process/', include('aps_process.urls')),
    )

Before your tags/filters are available in your templates, load them by using

.. code-block:: html

	{% load aps_process_tags %}


Don't forget to migrate your database

.. code-block:: bash

    ./manage.py migrate aps_process


Usage
-----

TODO: Describe usage or point to docs. Also describe available settings and
templatetags.


Contribute
----------

If you want to contribute to this project, please perform the following steps

.. code-block:: bash

    # Fork this repository
    # Clone your fork
    mkvirtualenv -p python2.7 django-aps-process
    make develop

    git co -b feature_branch master
    # Implement your feature and tests
    git add . && git commit
    git push -u origin feature_branch
    # Send us a pull request for your feature branch
