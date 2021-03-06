
Rapidsms_Dev
========================

Below you will find basic setup instructions for the ``rapidsms_dev``
project. To begin you should have the following applications installed on your
local development system:

- `Python >= 2.7 (including Python 3) <http://www.python.org/getit/>`_
- `pip >= 7.0.3 <http://www.pip-installer.org/>`_
- `virtualenv >= 13.0.3 <http://www.virtualenv.org/>`_

Getting Started
---------------

To setup your local environment you should create a virtualenv and install the
necessary requirements::

    virtualenv rapidsms_dev-env

On Posix systems you can activate your environment like this::

    source rapidsms_dev-env/bin/activate

On Windows, you'd use::

    rapidsms_dev-env\Scripts\activate

Then::

    cd rapidsms_dev
    pip install -U -r requirements/base.txt

Run migrate::

    python manage.py migrate

You should now be able to run the development server::

    python manage.py runserver
