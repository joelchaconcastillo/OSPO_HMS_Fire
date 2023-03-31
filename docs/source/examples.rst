Examples
=====

My Title
*********

Example 1 - Retrieving information given a startdate and enddate
---------------- 

The format of dates is ``Year-Month-Day``, 

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   example1

Example 2 Retrieve informatio given a satellite
---------------- 

.. code-block:: python

   data[data.Satellite=='NOAA 20']

Example 3 Plotting fires
---------------- 

.. code-block:: python

   HMSF.plot(points=data[data.Satellite=='NOAA 20'], minlon=-125, minlat=25, maxlon=-60, maxlat=50)
   HMSF.plot(points=data[data.Satellite=='GOES-EAST'], minlon=-125, minlat=25, maxlon=-60, maxlat=50)
   
Example 4 Pre-loaded bounding box of fires
---------------- 

.. code-block:: python

   print(HMSF.satelites())


Example 5 Retrieve the available satellites
---------------- 

.. code-block:: python

   print(HMSF.satelites())


Example 6 Pre-loaded bounding box of fires
---------------- 

.. code-block:: python

   print(HMSF.satelites())


Example 7 Frequency of Fire Radiative Power
---------------- 

.. code-block:: python

   data[(data.FRP>0) & (data.FRP<150) & (data.YearDay>2023000)].FRP.plot.hist(bins=40)
   plt.suptitle("Fire Radiative Power (FRP)")

Example 8 Re-samping data on time
---------------- 

.. code-block:: python

   timedata = HMSF.resamplingTime(data=data[['Time', 'FRP']], freq='7D')
   plt.rcParams["figure.figsize"] = (20,5) #modify size of plot
   plt.plot(timedata['Time'], timedata['FRP'])
   plt.xlabel('Time')
   plt.ylabel('FRP')
   plt.show()
   
Example 9 conversion to Xarray 
---------------- 

.. code-block:: python

   xrdata  = HMSF.getXarray()
