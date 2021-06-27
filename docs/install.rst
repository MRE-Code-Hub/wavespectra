.. image:: _static/MO_Horiz_Primary_rgb.png
   :width: 150 px
   :align: right

============
Installation
============

Install from pypi
-----------------
.. code:: bash

   # Default install, miss some dependencies and functionality
   pip install git+ssh://git@github.com/metocean/wavespectra

   # Complete install
   pip install 'git+ssh://git@github.com/metocean/wavespectra.git#egg=wavespectra[extra]'

Install from sources
--------------------
Get the source code from Github_:

.. code:: bash

    git clone git@github.com:metocean/wavespectra.git

Install requirements. Navigate to the base root of wavespectra and execute:

.. code:: bash

   # Default install, miss some dependencies and functionality
   pip install -r requirements/default.txt

   # Also, for complete install
   pip install -r requirements/extra.txt

   # Also, for testing requirements
   pip install -r requirements/test.txt

Then install wavespectra:

.. code:: bash

   python setup.py install

Alternatively, to install in `development mode`_:

.. code:: bash

   pip install -e .

Running tests
--------------------

.. code:: bash

    # Running all tests
    py.test -v

    # Or, alternatively
    python setup.py test

    # Running specific tests
    py.test -v tests/core
    py.test -v tests/core/test_wave_stats.py
    py.test -v tests/core/test_wave_stats.py::TestSpecArray

.. _Github: https://github.com/metocean/wavespectra
.. _development mode: https://pip.pypa.io/en/latest/reference/pip_install/#editable-installs
