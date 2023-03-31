Installation
=====

.. _installation:

Installation
------------

To use HMSFirepy, first install it using pip:

.. code-block:: console

   $ pip install HMSFire
   

Small example
----------------

To retrieve information of fires setting a ``startDate`` and ``endDate``

For example:

.. code-block:: console

   from OSPO.HMSFire import HMSF
   Fires = HMSF.HMSFire(startDate='2023-01-01', endDate='2023-02-01')
   data = Fires.getDataFrame()
   Fires.plot()
   print(Fires.satelites())
   Fires.plot(minlon=-125, minlat=25, maxlon=-60, maxlat=50)
   minlon, minlat, maxlon, maxlat = Fires.getBoundingBoxCounty(county='Dallas')
   Fires.plot(minlon=minlon, minlat=minlat, maxlon=maxlon, maxlat=maxlat)
   minlon, minlat, maxlon, maxlat = Fires.getBoundingBoxState(state='Texas')
   Fires.plot(minlon=minlon, minlat=minlat, maxlon=maxlon, maxlat=maxlat)
   
