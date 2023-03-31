Examples
=====

Example 1 - Retrieving information given a startdate and enddate
---------------- 

The format of dates is ``Year-Month-Day``, 
   
.. code-block:: python

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
   
Example 2 Plotting fires
---------------- 


Example 3 Pre-loaded bounding box of fires
---------------- 

Example 4 Retrieve the available satellites
---------------- 

Example 5 Pre-loaded bounding box of fires
---------------- 

Example 6 Retrieve informatio given a satellite
---------------- 

Example 7 Frequency of Fire Radiative Power
---------------- 

Example 8 Re-samping data on time
---------------- 

Example 9 conversion to Xarray 
---------------- 
