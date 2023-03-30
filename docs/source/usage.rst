Usage
=====

.. _installation:

Installation
------------

To use HMSFirepy, first install it using pip:

.. code-block:: console

   (.venv) $ pip install HMSFirepy

Creating recipes
----------------

To retrieve information of fires setting a ``startDate`` and ``endDate``

For example:
.. code-block:: console
   import HMSFirepy
   HMSF = HMSFire(startDate='2020-01-01', endDate='2023-02-01')
   print(HMSF.getDataFrame())
   HMSF.plot()

