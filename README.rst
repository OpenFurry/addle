=====
Addle
=====

|Build Status| |Coverage Status| |PyPI|

Pluggable advertisement and promotion managing application

Quick start
-----------

1. Add "addle" to your INSTALLED_APPS setting like this::

    INSTALLED_APPS = [
        ...
        'addle',
    ]

   Ensure that you have `django.contrib.auth` added as an application as well.

2. Include the addle URLconf in your project urls.py like this::

    url(r'^addle/', include('addle.urls')),

3. Run ``python manage.py migrate`` to create the addle models.

4. Start the development server.

5. Visit http://127.0.0.1:8000/addle/ to see the app.

Notes for the pluggable application
-----------------------------------

The standalone application is basically ready to use as one would normally run
a Django app, but the pluggable application has a few more things to note.

- Addle hooks into the Django permissions system. (...)
- Addle is designed, loosely, for a site using `Bootstrap
  <https://getbootstrap.com>`__, so elements are classed as such, but this is
  designed to not be a hard requirement.  To that end, some styles are defined within the templates.

Further information
-------------------

Source, issues, and further information:
  `GitHub <https://github.com/OpenFurry/addle>`__
Author
  `The OpenFurry Contributors <http://OpenFurry.org>`__

.. |Build Status| image:: https://travis-ci.org/OpenFurry/addle.svg?branch=master
   :target: https://travis-ci.org/OpenFurry/addle
.. |Coverage Status| image:: https://coveralls.io/repos/github/OpenFurry/addle/badge.svg?branch=master
   :target: https://coveralls.io/github/OpenFurry/addle?branch=master
.. |PyPI| image:: https://img.shields.io/pypi/v/django-addle.svg
   :target: https://pypi.python.org/pypi/django-addle/
