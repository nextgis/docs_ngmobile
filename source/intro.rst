.. sectionauthor:: Dmitry Baryshnikov <dmitry.baryshnikov@nextgis.ru>

.. _ngmob_intro:

Introduction
=============

.. _ngmob_purpose:

About the Gramrekha GIS App
------------------------

**Gramrekha Mobile** - is a mobile :abbr:`GIS (Geographic Information System)` for :term:`Android` OS.

Gramrekha Mobile allows to:

* display a map from a set of layers;
* perform map navigation (zoom in, zoom out, pan);
* add vector data from :term:`GeoJSON` format;
* add cached raster data in zip archive;
* add online tile sources (:term:`XYZ` and :term:`TMS`);
* add raster and vector layers from `Gramrekha Web <http://gramrekha.com/>`_;
* create and modify vector :term:`geodata` (geometries and attributes);
* browse the attributes of selected geometry through identify dialog;
* modify the attributes of vector layer with customizable input forms;
* share the resultant vector data locally or in the cloud with variety of Apps;
* record the tracks and manage their display parameters, remove selected or all tracks;
* display coordinates, velocity, altitude of device on the map, as well as a source of geographical coordinates and amount of satellites used for georeferencing (if :term:`GPS` is used);
* collect and transmit to `Gramrekha Web <http://gramrekha.com>`_ created and/or edited :term:'geodata' in background mode (when internet connection is on).

Gramrekha Mobile is open source
(license :ref:`GPL v3 <ngmobile_gplv3>`).

Some icons used in Gramrekha Mobile are from:

* `Icons8.com <http://icons8.com/android-icons>`_ distributed on `CC BY-ND 3.0 <http://creativecommons.org/licenses/by-nd/3.0/>`_;
* `romannurik.github.io <http://romannurik.github.io/AndroidAssetStudio/icons-launcher.html>`_ - `CC BY 3.0 <http://creativecommons.org/licenses/by/3.0/>`_.

.. only:: latex

   This documentation is distributed under Creative Commons license
	**"Attribution-NoDerivs" ("Attribution - without derivative works") СC BY-ND**
   
   .. image:: _static/cc_by.png  

Documentation is describing Gramrekha Mobile version 2.5.

 
.. _ngmobile_launch_conditions:

Hardware and Software requirements
-------------------------------------

To launch Gramrekha Mobile you need a device (smartphone, tablet, etc.) with :term:`Android` 4.4 or higher.

To be able to use all Gramrekha Mobile features the device should have the following hardware:

* :term:`GPS` and/or :term:`GLONASS` sensor;
* digital compass;
* cellular module;
* rear camera.

.. note::

   If any of these items are missing from the device, the related functions will not be available.

Gramrekha Mobile does not impose specific system requirements. However, the amount of system memory and storage space can limit the size of uploaded geodata.
