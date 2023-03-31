Installation
=====

.. _installation:

pip installation
------------

To use HMSFirepy, first install it using pip:

.. code-block:: console

   $ pip install HMSFire
   

Technical requirements
----------------
This package has dependencies with the modules:

* basemap.
* pandas.
* matplotlib.
* requests.
* datetime.

.. warning :
   In this preliminary version each query will download each day fire information, therefore larger ranges of time will require download a large amount of information. 


Test
----------------

To retrieve information of fires at least is needed a ``startDate`` and ``endDate``

For example:

.. code-block:: console

   from OSPO.HMSFire import HMSF
   Fires = HMSF.HMSFire(startDate='2023-01-01', endDate='2023-02-01')
   data = Fires.getDataFrame()
   print(data)
   Fires.plot()   
