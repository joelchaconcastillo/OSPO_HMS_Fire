Hazard Mapping System Fire (HMSFirepy) documentation
===================================
**HMSFirepy** make searching, downloading and retrieving data of the Hazard Mapping System easy (https://www.ospo.noaa.gov/Products/land/hms.html#maps/)

This package is developmed as an effor to offer data more accessible outside the atmospheric scientific community.

It offers an easy-to-use class, thus this 

About Hazard Mapping System Fire
===================================

Users should note:

The initial HMS product for the current day is created and updated by a satellite analyst roughly between 8am and 10am Eastern Time. After 10am, the analysis is fine-tuned as time permits as additional satellite data becomes available. The product is finalized and "completed" for the archive the following morning - generally by around 8am.
The fire sizes depicted in the product are primarily determined by the field of view of the satellite instrument, or the resolution of the analysis tool. They should not be used to estimate specific fire perimeters.

Satellite fire detection data are displayed using a color scheme based on the pixel's fire radiative power (FRP), given in MegaWatts [MW]). Higher FRP values may describe the most active portion of a fire pixel cluster at the moment of observation, whereas absolute values can be greatly influenced by imaging conditions. A fill value of -999 is used when no FRP retrieval is available.

The ability to detect fires and smoke can be compromised by many factors, including cloud cover, tree canopy, terrain, the size of the fire or smoke plume, the time of the day, etc. The satellite sensors used to detect fires are sensitive to heat sources and reflected sunlight. Analysts do their best to distinguish between fires and other heat sources or highly reflective surfaces, such as factories, mines, gas flares, solar panels, clouds, etc. but some false detects do get included in the analysis.

More information can be reviewed at https://www.ospo.noaa.gov/Products/land/hms.html#about 

Check out the :doc:`usage` section for further information, including
how to :ref:`installation` the project.

.. note::

   This project is under active development.

Contents
--------

.. toctree::

   usage
   api
   examples
