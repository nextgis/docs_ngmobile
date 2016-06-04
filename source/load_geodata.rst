.. sectionauthor:: Дмитрий Барышников <dmitry.baryshnikov@nextgis.ru>

.. _ngmobile_load_geodata:

Add layer
============

NextGIS Mobile has the ability to add data from local storage, cloud storage or 
mobile devices storage and also to create new empty vector layer. Types of local storage data: 
GeoJSON, cached tiles, custom forms.

New layer
---------

.. versionadded:: 2.3

Here are the steps to create an empty vector layer:

1. Open options menu and select "New Layer", then select "Create Layer" (see :numref:`ngmobile_options_menu_new_layer_pic`)

.. figure:: _static/options_menu_new_layer.png
   :name: ngmobile_options_menu_new_layer_pic
   :align: center
   :height: 10cm
 
   Options menu.

2. In the attributes window you need to add fields for new vector layer (see :numref:`ngmobile_input_form_attributes_new_layer_pic`) 

.. figure:: _static/input_form_attributes_new_layer.png
   :name: ngmobile_input_form_attributes_new_layer_pic
   :align: center
   :height: 10cm
   
   Attributes for new vector layer.

The standard attributes form of a new vector layer has the following field to fill:

1. Name of a layer - enter the name of layer which will be displayed in layers tree.
2. Geometry type - choose geometry type (point, linestring, polygon, multypoint, multilinestring or multipolygon).
3. Fields - list of fields, can be added, edited or deleted.

New dialog will be opened for each field in the menu of standard attributes form (see :numref:`ngmobile_dialogue_create_new_field_pic`) 

.. figure:: _static/dialogue_create_new_field.png
   :name: ngmobile_dialogue_create_new_field_pic
   :align: center
   :height: 10cm

   Dialog of the new field creation.

New dialog consists of the following fields:

1. Field name – the name of the field.

.. note:: 
	The field name can only be entered in Latin characters (letters and numbers!) without spaces. It should also be different from the official words of SQL.

2. Field type - select field type (string, integer, real, date&time, date, time)


GeoJSON
-------

To open data in GeoJSON format:

1. Open options menu, select "New layer" and choose option "Open local" (see :numref:`ngmobile_add_ngw_layer_geo_pic`)

.. figure:: _static/add_layer1.png
   :name: ngmobile_add_ngw_layer_geo_pic
   :align: center
   :height: 10cm
    
    Adding local layer.

2. Select the GeoJSON format file stored on your mobile device drive that you want to open (see :numref:`ngmobile_saved_files_on_the_drive_unit_pic`): 

.. figure:: _static/saved_files_on_the_drive_unit.png
   :name: ngmobile_saved_files_on_the_drive_unit_pic
   :align: center
   :height: 10cm
   
   Android file listing.


3. After selecting the file a dialog with layer settings will open. Here you can specify layer's name. (see :numref:`ngmobile_layer_settings_geo_pic`): 

.. figure:: _static/layer_settings_geo.png
   :name: ngmobile_layer_settings_geo_pic
   :align: center
   :height: 10cm

   Settings for created layer.

4. "Create" starts the process of data processing for a new layer (see :numref:`ngmobile_processing_and_creation_layer_pic`): 

.. figure:: _static/processing_and_creation_layer.png
   :name: ngmobile_processing_and_creation_layer_pic
   :align: center
   :height: 10cm  

   Creation and data processing for a new layer.

.. note::  
	In the case of loading GeoJSON format file in the app new geodata layer type will be a vector always!

You can check a presence or absence of the layer in the layers tree. If new layer was successfuly created it will show up first in the layers tree (see :numref:`ngmobile_tree_layers_geo_pic`):

.. figure:: _static/tree_layers_geo.png
   :name: ngmobile_tree_layers_geo_pic
   :align: center
   :height: 10cm  

   Layers tree.

*GeoJSON: format requirements*

* :term:`Coordinate system` of input geometries can be WGS 84 (EPSG:4326) or Web Mercator (EPSG:3857) only. If input file has different coordinate system you will see a warning message about unsupported coordinate system.
* Geometries in the file must be all of the same type. If input file contains varying types of geometry, in the output you will have a file with geometries type that coincides with the type of first record, i.e. geometry of first entry will determine the type of layer geometry.
* Text strings must be encoded in UTF-8 format.

.. note::
	You can read more about the GeoJSON format can in its `specification <http://geojson.org/>`_.
	GeoJSON is based on the format JSON (see `RFC 4627 <https://www.ietf.org/rfc/rfc4627.txt>`_).

A feature of vector layer editing while loading GeoJSON format is a procedure of filling the standard form of attributes. It contains the following fields:

1. Text field for entering characters or digits.
2. Dialog of enter and time.
3. Add pictures and recording button.

An example of standard form for editing attributes :numref:`ngmobile_standard_form_layer_attributes_pic`: 

.. figure:: _static/standard_form_layer_attributes.png
   :name: ngmobile_standard_form_layer_attributes_pic
   :align: center
   :height: 10cm  
    
    Standard form for editing attributes.

For more information about editing a GeoJSON layer, see section :ref:`ngmobile_editing`.

Tile cache
----------

Tile cache is a zip file with folders and tiles stored in accordance with a tiling scheme (for example, folder_z/folder_x/y.png). Folders of level Z can be located in the root or in a folder in the root folder (name of the folder can be any, but there have to be only one folder). Deeper nesting of level Z folders is not allowed.

Follow these steps to open zip archive with tiles:

1. Open options menu and select "New layer", than choose "Open local"  (see :numref:`ngmobile_add_ngw_layer_geo_pic`) 

2. In the opened window select the zip file stored in your mobile device's memory (see :numref:`ngmobile_files_on_the_drive_unit_tms_pic`): 

.. figure:: _static/files_on_the_drive_unit_tms.png
   :name: ngmobile_files_on_the_drive_unit_tms_pic
   :align: center
   :height: 10cm
   
   Android file listing.

3. Settings dialog for adding a layer will be opened after selecting zip file. Here you can choose type of tile layer (tile structure system) - XYZ (OSM) or TMS (OSGeo) (see :numref:`ngmobile_layer_setting_tms_pic`):

.. figure:: _static/layer_setting_tms.png
   :name: ngmobile_layer_setting_tms_pic
   :align: center
   :height: 10cm

   Tile layer settings

4. "Create" button will start new layer creation (see :numref:`ngmobile_processing_and_creation_layer_tms_pic`): 

.. figure:: _static/processing_and_creation_layer_tms.png
   :name: ngmobile_processing_and_creation_layer_tms_pic
   :align: center
   :height: 10cm  

Processing and creation of a layer from tiles.

If process was successful new tile layer should appear in the layers tree (see :numref:`ngmobile_tree_layers_tms_pic`):  

.. figure:: _static/tree_layers_tms.png
   :name: ngmobile_tree_layers_tms_pic
   :align: center
   :height: 10cm  

   Layers tree menu.


Custom forms
------------

.. versionadded:: 2.2

NGFP file format can be generated with NextGIS FormBuilder. NGFP is a :term:`GeoJSON` file with additional information (JSON) which is packaged in zip archive and has ngfp extension.

Perform the following steps to add NGFP file to NextGIS Mobile:

1. Select "New layer" in options menu and choose "Open local" (see :numref:`ngmobile_add_ngw_layer_geo_pic`) 

2. Select the NGFP file that you want to open from your mobile device's memory (see :numref:`ngmobile_files_on_the_drive_unit_tms_pic`)

3. After selecting NGFO file settings dialog for a new layer will open. Here you can type a name for the new layer (see :numref:`ngmobile_settind_layer_form_pic`): 

.. figure:: _static/settind_layer_form.png
   :name: ngmobile_settind_layer_form_pic
   :align: center
   :height: 10cm

   Settings for a new layer.

4. "Create" will start processing for a new layer (see :numref:`ngmobile_loading_layer_form_pic`): 

.. figure:: _static/loading_layer_form.png
   :name: ngmobile_loading_layer_form_pic
   :align: center
   :height: 10cm  

   New layer’s creation.

A feature of NGFP layer is a custom attributes form optimized for viewing and editing. Custom form can contains special  controls for editing such as dropdowns, checkboxes or linked lists.


An example of a custom form attributes form:numref:`ngmobile_non-standard_form_pic`: 

.. figure:: _static/non-standard_form.png
   :name: ngmobile_non-standard_form_pic
   :align: center
   :height: 10cm  
    
    Custom form of layer attributes editor.

More information about editing NGFP can be found in section :ref:`ngmobile_editing`.

Adding tile service
-------------------

"Add web" from new layer menu (see :numref:`ngmobile_main_activity_pic` p. 3) opens the following dialog :numref:`ngmobile_add_tms_pic`.

.. figure:: _static/ngmobile_addtms.png
   :name: ngmobile_add_tms_pic
   :align: center
   :height: 11cm
   
   Dialog of adding tile geodata source.

   The numbers indicate: 1 - layer name; 2 - layer URL; 3 - tile layer type; 4 - login; 5 - password; 6 - create new layer button; 7- cancel.

Address of tile server should specify location of X value (number of tile by horizontal), Y (number of tile by vertical) and Z (zoom level). These values are specified using wildcard code for X - **{x}**, for Y - **{y}**, for Z - **{z}**. Additionally you can specify subdomains (eg, for subdomains a.tileopenstreetmap.org, b.tileopenstreetmap.org, c.tileopenstreetmap.org. The address will look like this: **{a,b,c}.tile.openstreetmap.org**).

.. note::

	Application requests tiles from each address (subdomain) in two streams. So for an address {a,b,c}.tile.openstreetmap.org NextGIS Mobile will download tiles in 6 streams.

All tiles received from Internet/Intranet are cached on memory card. When you request a specific tile, local cache is first checked. If there is a tile in the local cache and its creation time at least seven days, then it will be displayed on the map. Cached tile will also be displayed when there is no connection to the Internet/Intranet, or if there was a failure while getting a tile. Tiles obtained from the Internet/Intranet will replace tiles in the cache.

Following choices are available in the list of types of tile layers (see :numref:`ngmobile_add_tms_pic`, p. 3):

* XYZ (OSM) - standard type of tile service;
* TMS (OSGeo) - OSGeo standard.

If authentication is required for accessing tiles, you can specify a username and password.

.. note::

	Only `Basic access authentication <http://en.wikipedia.org/wiki/Basic_access_authentication>`_ is currently available.

Caching of tile service data 
----------------------------

.. versionadded:: 2.2

Image layer is using :term:`tiles <tile>` received from Internet and cached on memory card of the device. Cached tiles are  available without Internet connection.
To pre-load tiles for current map extent select "Download tiles" (see :numref:`ngmobile_levels_of_zoom_pic`):

.. figure:: _static/levels_of_zoom.png
   :name: ngmobile_levels_of_zoom_pic
   :align: center
   :height: 10cm
 
 	Selecting zoom levels to download tiles.

The lower selected zoom level for downloading of tiles, the smaller number of tiles will have to be downloaded for an area of interests and faster downloading of whole tile cache will be.

.. note::
	If the list of tiles to download for a given zoom levels is greater than 1000 tiles, only first 1000 tiles will be downloaded. The rest will not be downloaded due to danger for memory overflow.

After setting up required zoom levels you can start downloading tiles by pressing "Start" button. Download process will be moved to the status bar of your phone. You can stop downloading by pressing button "Stop" in the status bar menu (see :numref:`ngmobile_loading_tiles_in_the_status_bar_pic`):


.. figure:: _static/loading_tiles_in_the_status_bar.png
   :name: ngmobile_loading_tiles_in_the_status_bar_pic
   :align: center
   :height: 10cm

   Loading tiles in the status bar.

