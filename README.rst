===============
Crontab Manager
===============

Crontab Manager is a Django app that aims to help manage cronjobs running by `django-crontab <https://pypi.org/project/django-crontab>`. 

Detailed documentation is in the "docs" directory.

Quick start
===========
1. install via pip:

.. code:: bash

    pip install django-crontab-manager

2. Add "django_crontab_manager" and the "django_crontab" to your INSTALLED_APPS setting like this:

.. code:: bash

    pip install django-crontab

    INSTALLED_APPS = [
        ...
        'django_crontab',
        'django_crontab_manager'
    ]

3. Include the polls URLconf in your project urls.py like this:

.. code:: bash    
    
    path('crontab_manager/', include('crontab_manager.urls')), 

4. Access the management dashboard at the URL http://127.0.0.1:8000/crontab_manager/.

license
=======
MIT-License, see LICENSE file.