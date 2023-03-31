Examples
=====

.. Example 1 Retrieving information given a startdate and enddate:
   
   
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
   
.. Example 2 Plotting fires

.. Example 3 Pre-loaded bounding box of fires

.. Example 4 Retrieve the available satellites

.. Example 5 Pre-loaded bounding box of fires

.. Example 6 Retrieve informatio given a satellite

.. Example 7 Frequency of Fire Radiative Power

.. Example 8 Re-samping data on time

.. Example 9 conversion to Xarray 


.. code-block:: console

   (.venv) $ pip install lumache

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``lumache.get_random_ingredients()`` function:

.. autofunction:: lumache.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`lumache.get_random_ingredients`
will raise an exception.

.. autoexception:: lumache.InvalidKindError

For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']
