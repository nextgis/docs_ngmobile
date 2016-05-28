.. sectionauthor:: Дмитрий Барышников <dmitry.baryshnikov@nextgis.ru>

.. _ngmobile_intro:

Introduction
============

.. _ngmob_purpose:

Purpose of the program
----------------------

**NextGIS Mobile** - is a mobile :term:`geographic information system` (:abbr:`GIS`) for operating system :term:`Android`.

GIS NextGIS Mobile allows to:

* display a map from a set of layers;
* perfom map navigation (zoom in, zoom out, roam);
* add vector data from :term:`GeoJSON` format;
* add cached raster data in zip archive;
* add online tile sources (XYZ and :term:`TMS`);
* add raster and vector layers from NextGIS Web;
* create and modify vector :term:`geodata` (geometry and attributes);
* browse the attributes of selected geometry through identify dialog;
* modify the attributes of vector layer with customizable input forms;
* record the tracks and manage their display parameters, remove selected tracks or all tracks;
* display coordinates, velocity, altitude of device on the map, source of geographical coordinates, amount of satellites which are used for georeferencing (in the case of :term:`GPS`);
* collect and transmit in backround mode by Internet (when connected) in the NextGIS Web created and/or edited :term:'geodata' from vector layers.

NextGIS Mobile is open source
(license :ref:`GPL v3 <ngmobile_gplv3>`).

Some icons used in application are from:

* `Icons8.com <http://icons8.com/android-icons>`_ distributed on `CC BY-ND 3.0 <http://creativecommons.org/licenses/by-nd/3.0/>`_;
* `romannurik.github.io <http://romannurik.github.io/AndroidAssetStudio/icons-launcher.html>`_ - `CC BY 3.0 <http://creativecommons.org/licenses/by/3.0/>`_.

.. only:: latex

   This documentation is distributed under Creative Commons license
	**"Attribution-NoDerivs" ("Attribution - without derivative works") СC BY-ND**
   
   .. image:: _static/cc_by.png  

Documentation is describing NextGIS Mobile version 2.2. Newer versions of NextGIS Mobile might be currently available.

 
.. _ngmobile_launch_conditions:

Launch conditions
-------------------------

To launch NextGIS Mobile you need version 2.2 or higher :term: `Android` device (smartphone, tablet, etc.). 
The device might have the following equipment:

* sensor :term:'GPS' and/or :term:'GLONASS';
* digital compass;
* cellular module;
* rear camera.

.. note::

   If any on these items are missing from the device, the related functions will not be available.

NextGIS Mobile does not impose specific system requirements, however, the amount of system memory and storage space can limit the size of uploaded geodata.
