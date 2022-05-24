.. sectionauthor:: Dmitry Baryshnikov <dmitry.baryshnikov@nextgis.ru>, Abhay Kulkarni <praxisnfp@gmail.com>

.. _ngmob_intro:

Introduction
=============

.. _ngmob_purpose:

About NextGIS Mobile
------------------------

**NextGIS Mobile** is a mobile :abbr:`GIS (Geographic Information System)` for :term:`Android` OS.

NextGIS Mobile allows to:

* create and display a multi-layered map;
* perform map navigation (panning, zooming in and out);
* add vector data in :term:`GeoJSON` format;
* add raster data as a tile cache;
* add online tile sources (:term:`XYZ` and :term:`TMS`);
* add raster and vector layers from `nextgis.com <https://my.nextgis.com/signup/?next=/webgis/>`_ and `NextGIS Web <http://nextgis.com/nextgis-web/>`_;
* create and modify vector :term:`geodata` (geometries and attributes);
* browse the attributes of selected geometry through identify dialog;
* modify vector layer attributes with customizable input forms;
* share vector geodata using standard Android tools;
* record the tracks and manage their display parameters, remove selected or all tracks;
* display device coordinates, velocity, altitude on the map, as well as a source of geographical coordinates and amount of satellites used for georeferencing (when :term:`GPS` is in use);
* collect :term:`geodata` and transmit it to `nextgis.com <https://my.nextgis.com/signup/?next=/webgis/>`_ or `NextGIS Web <http://nextgis.com/nextgis-web/>`_ in background mode (when internet connection is on).

NextGIS Mobile is open source
(license :ref:`GPL v3 <ngmobile_gplv3>`).

Some icons used in NextGIS Mobile are from:

* `Icons8.com <http://icons8.com/android-icons>`_ distributed on `CC BY-ND 3.0 <http://creativecommons.org/licenses/by-nd/3.0/>`_;
* `romannurik.github.io <http://romannurik.github.io/AndroidAssetStudio/icons-launcher.html>`_ - `CC BY 3.0 <http://creativecommons.org/licenses/by/3.0/>`_.

.. only:: latex

   This documentation is distributed under Creative Commons license
	**"Attribution-NoDerivs" ("Attribution - without derivative works") СC BY-ND**
   
   .. image:: _static/cc_by.png  

This documentation describes NextGIS Mobile 2.5. 

 
.. _ngmobile_launch_conditions:

Hardware and software requirements
-------------------------------------

To launch NextGIS Mobile you need a device (smartphone, tablet, etc.) with :term:`Android` **5.0** or higher.

To be able to use all NextGIS Mobile features the device should have the following hardware:

* :term:`GPS` and/or :term:`GLONASS` sensor;
* digital compass;
* cellular module;
* rear camera.

.. note::

   If any of these items are missing from the device, the related functions will not be available.

NextGIS Mobile does not impose specific system requirements. However, the amount of system memory and storage space can limit the size of uploaded geodata.
