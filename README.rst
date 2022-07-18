================
django-couchbase (for Django > 4.0)
================

This package is aimed at developing the ORM for the couchbase - the next generation NoSQL database.

Updated to run on newer versions of Django


Dependencies
------------

Make sure you install the below dependencies::

    couchbase==4.0.2
    shortuuid==0.4.3
    six==1.16.0
    django-extensions==3.2.0
    django-tastypie==0.14.4

Quick Install
-------------

Install django-couchbase package::

    pip install django-couchbase

The following configuration settings are used for the package (you can use the set below for the fast installation)::


    CB_BUCKETS = {
        "MAIN_BUCKET" : {
            'HOST': 'localhost',
            'USER': 'USER_NAME',
            'PASSWORD': 'PASSWORD',
            'BUCKET': 'BUCKET_NAME',
            'SCOPE': '_default',
            'COLLECTION': '_default'
        }
    }
}

Add ``django_couchbase`` to ``INSTALLED_APPS``::

    INSTALLED_APPS = (
        # ...
        'django_couchbase',
    )

