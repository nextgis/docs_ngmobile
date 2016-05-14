.. sectionauthor:: Дмитрий Барышников <dmitry.baryshnikov@nextgis.ru>

.. _ngmobile_intro:

Introduction
============

.. _ngmobile_purpose:

Purpose of the program
----------------------

**NextGIS Mobile** - is a mobile :term:`geographic information system` (:abbr:`GIS`) for operating system :term:`Android`.

GIS NextGIS Mobile allows to:

* display the map as a set of layers;
* perfom navigation by map (zoom in, zoom out, roam);
* add the vector data from :term:`GeoJSON` format;
* add cached raster data in zip archive;
* connect online source of tiles (XYZ and :term:`TMS`);
* connect raster and vector layers from NextGIS Web;
* create and modify vector :term:`geodata' (geometry and attributes);
* browse the attributes of selected geometry through identify dialog;
* modify the attributes of vector layer by customizable forms of input;
* record the tracks and manage their display, and also remove selected tracks or all tracks;
* display coordinates, velocity, altitude of device on the map, source of geographical coordinates, amount of satilates wich are used for georeferencing (in the case of :term:`GPS`);
* collect and transmit in backround mode by Internet (when connected) in the NextGIS Web created and/or edited :term:'geodata' from vector layers.


NextGIS Mobile - is a software with open source code
(license :ref:`GPL v3 <ngmobile_gplv3>`).

Some icons which are used in application received from this web sites:

* `Icons8.com <http://icons8.com/android-icons>`_ distributed on `CC BY-ND 3.0 <http://creativecommons.org/licenses/by-nd/3.0/>`_;
* `romannurik.github.io <http://romannurik.github.io/AndroidAssetStudio/icons-launcher.html>`_ - `CC BY 3.0 <http://creativecommons.org/licenses/by/3.0/>`_.

.. only:: latex

   This documentation is distributed by Creative Commons license
	**"Attribution-NoDerivs" ("Attribution - without derivative works") СC BY-ND**
   
   .. image:: _static/cc_by.png  

Documentation is describing NextGIS Mobile version 2.2.

 
.. _ngmobile_launch_conditions:

Program launch condition
---------------------------

To launch the program you need the device (smartphone, tablet, etc.) under the operating system: term: `Android` version 2.2 ** ** or higher 
The device should be equipped with the following equipment:

* sensor :term:'GPS' and/or :term:'GLONASS';
* digital compass;
* cellular module;
* rear camera.

.. note::

   If any items are missing from the equipment in the device, the related functions are not available.

The program does not impose specific system requirements, however, the amount of memory and memory for storing data can limit the size of uploaded geodata on a map.
