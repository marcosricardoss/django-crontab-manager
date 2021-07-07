===============
Crontab Manager
===============

Crontab Manager is a Django app that aims to help manage cronjobs running by `django-crontab <https://pypi.org/project/django-crontab>`_. 

Detailed documentation is in the "docs" directory.

setup
=====
Install via pip:

.. code:: bash

    pip install django-crontab-manager

Add "django_crontab_manager" and the "django_crontab" to your INSTALLED_APPS setting like this:

.. code:: bash

    pip install django-crontab

    INSTALLED_APPS = [
        ...
        'django_crontab',
        'django_crontab_manager'
    ]

Include the polls URLconf in your project urls.py like this:

.. code:: bash    
    
    path('crontab_manager/', include('crontab_manager.urls')), 

Access the management dashboard at the URL http://<your-url-project>/crontab_manager/.

license
=======
MIT-License, see LICENSE file.