=============================
Django Rest Framework Msgpack
=============================

.. image:: https://api.travis-ci.org/juanriaza/django-rest-framework-msgpack.png?branch=master

:Version: 1.0.0
:Author: `Juan Riaza <http://juanriaza.com>`_

Overview
========

`MessagePack <http://msgpack.org>`_ is a fast, compact binary serialization format, suitable for similar data to JSON.
This package provides `MessagePack <http://msgpack.org>`_ support for `Django REST framework <http://django-rest-framework.org>`_.

How to install
==============

Install using ``pip``::

    $ pip install djangorestframework-msgpack

...or clone the project from github::

    $ git clone git@github.com:juanriaza/django-rest-framework-msgpack.git
    $ cd django-rest-framework
    $ pip install -r requirements.txt

How use it?
===========

This package provides a renderer ``MessagePackRenderer`` and a parser ``MessagePackParser``.

Setting the renderer and the parser
-----------------------------------

Just follow the documentation:

- `Setting the renderer <http://django-rest-framework.org/api-guide/renderers.html#setting-the-renderers>`_.
- `Setting the parser <http://django-rest-framework.org/api-guide/parsers.html#setting-the-parsers>`_.


``rest_framework_msgpack.renderers.MessagePackRenderer``
---------------------------------------------------------

Renders the request data into ``MessagePack``.

:.media_type: ``application/msgpack``
:.format: ``.msgpack``

``rest_framework_msgpack.parsers.MessagePackParser``
---------------------------------------------------------

Parses ``MessagePack`` request content.

:.media_type: ``application/msgpack``


Running the tests
=================

To run the tests against the current environment::

    ./manage.py test

Changelog
=========

1.0.0
-----

* Initial release