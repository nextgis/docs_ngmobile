.. sectionauthor:: Dmitry Baryshnikov <dmitry.baryshnikov@nextgis.ru>

.. _ngmobile_load_geodata:

Adding layers
==============

NextGIS Mobile has the ability to create layers using data from cloud storage or 
mobile device storage and also to create new empty vector layers. Supported data types: 
GeoJSON, cached tiles, custom forms.

Creating new vector layer
---------------------------
  
.. versionadded:: 2.3

Here are the steps to create an empty vector layer:

1. First tap on "Layers tree menue" (item 1 in :numref:`ngmobile_main_activity_pic_1`). Then tap on "Add geodata" (item 4 in :numref:`ngmobile_layer_tree_pic`) and select "Create layer" (see :numref:`ngmobile_options_menu_new_layer_pic`)

.. figure:: _static/options_menu_new_layer.png
   :name: ngmobile_options_menu_new_layer_pic
   :align: center
   :height: 10cm
 
   Add geodata Contextual menu.

2. In the opened dialog enter the parameters of new vector layer (see :numref:`ngmobile_input_form_attributes_new_layer_pic`) 

.. figure:: _static/input_form_attributes_new_layer.png
   :name: ngmobile_input_form_attributes_new_layer_pic
   :align: center
   :height: 10cm
   
   Parameters of the new vector layer.

The standard form for the creation of new vector layer contains the following parameters:

1. Layer name - enter the name of layer which will be displayed in layers tree.
2. Geometry type - select layer geometry type (point, linestring, polygon, multypoint, multilinestring or multipolygon).
3. Fields - list of fields which can be added, edited or deleted.

New dialog will be opened for creation of each field (see :numref:`ngmobile_dialogue_create_new_field_pic`) 

.. figure:: _static/dialogue_create_new_field.png
   :name: ngmobile_dialogue_create_new_field_pic
   :align: center
   :height: 10cm

   Dialog for creation of a new field.

Dialog for creation of a new field contains the following parameters:

1. Field name – enter the name of the field.

.. note:: 
	The field name can only be entered in Latin characters (letters and numbers!) without spaces. It should also differ from SQL reserved keywords.

2. Field type - select field type from one of the (string, integer, real, date&time, date, time)


Creating vector layer from GeoJSON data
-----------------------------------------

To open data in GeoJSON format:

1. First tap on "Layers tree menue" (item 1 in :numref:`ngmobile_main_activity_pic_1`). Then tap on "Add geodata" (item 4 in :numref:`ngmobile_layer_tree_pic`) and select "Open local" (see :numref:`ngmobile_options_menu_new_layer_pic`)

2. Select the GeoJSON dataset from your mobile device storage (see :numref:`ngmobile_saved_files_on_the_drive_unit_pic`). E.g. tap on the file "Roads.geojson". 

.. figure:: _static/saved_files_on_the_drive_unit.png
   :name: ngmobile_saved_files_on_the_drive_unit_pic
   :align: center
   :height: 10cm
   
   Android local storage.

3. When the file is selected a layer settings dialog opens. Here you can specify a layer name. (see :numref:`ngmobile_layer_settings_geo_pic`). E.g. "Roads". 

.. figure:: _static/layer_settings_geo.png
   :name: ngmobile_layer_settings_geo_pic
   :align: center
   :height: 10cm

   Layer settings dialog.

4. Pressing "Create" button starts data processing for creation of a new layer 

.. note::  
	In case of GeoJSON data uploading the new layer will always be a vector type layer!

You can check if the new layer was created successfully in the layers tree panel. The newly created layer will show up in the layers tree (see :numref:`ngmobile_tree_layers_geo_pic`). The "Roads" layer is shown in orange rectangle.

.. figure:: _static/tree_layers_geo.png
   :name: ngmobile_tree_layers_geo_pic
   :align: center
   :height: 10cm  

   Layers tree panel.

*GeoJSON: format requirements*

* :term:`Coordinate system` of input geometries can be WGS 84 (EPSG:4326) or Web Mercator (EPSG:3857) only. If input file has different coordinate system you will see a warning message about unsupported coordinate system.
* All geometries in the file must be of the same type. If input file contains varying types of geometry in the output you will have a file with geometries type that coincides with the type of first record, i.e. geometry of first entry will determine the type of layer geometry.
* Text strings must be encoded in UTF-8 format.

.. note::
	You can read more about the GeoJSON format in its `specification <http://geojson.org/>`_.
	GeoJSON is based on the format JSON (see `RFC 4627 <https://www.ietf.org/rfc/rfc4627.txt>`_).

You can only use standard attributes form for editing GeoJSON layer as against custom attributes form of ngfp format. Standard attributes form contains the following fields:

1. Text field for entering characters or digits.
2. Dialog for entering time.
3. "Add pictures and records" button.

.. figure:: _static/input_form_attributes.png
   :name: ngmobile_standard_input_form_attributes_pic
   :align: center
   :height: 10cm  
    
    Standard attributes form.

For more information about GeoJSON layer editing see :ref:`ngmobile_editing`.

Creating new raster layer from Tile cache (NGRC)
------------------------------------------------

Tile cache is a zip-archive with folders and tiles stored in accordance with a tiling scheme (for example, folder_z/folder_x/y.png) and compressed in a file having an extension ".ngrc". Folders of level Z can be located in the root or in a folder in the root folder (name of the folder doesn't matter, but there have to be only one folder). Deeper nesting of level Z folders is not allowed.

Follow these steps to open tile cached raster file in ngrc format:

1. First tap on "Layers tree menue" (item 1 in :numref:`ngmobile_main_activity_pic_1`). Then tap on "Add geodata" (item 4 in :numref:`ngmobile_layer_tree_pic`) and select "Open local" (see :numref:`ngmobile_options_menu_new_layer_pic`) 

2. Select ngrc file from your mobile device storage (see :numref:`ngmobile_saved_files_on_the_drive_unit_pic`). E.g. tap on the file name "Tandali_Wadgaon.ngrc" 

.. figure:: _static/saved_files_on_the_drive_unit.png
   :name: ngmobile_saved_files_on_the_drive_unit_pic
   :align: center
   :height: 10cm
   
   Android local storage.

3. You can check if the new layer was created successfully in the layers tree panel. The newly created layer will show up in the layers tree (see :numref:`ngmobile_tree_layers_ngrc_pic`). The "Tandali Wadgaon" layer is shown in orange rectangle.

.. figure:: _static/tree_layers_ngrc.png
   :name: ngmobile_tree_layers_ngrc_pic
   :align: center
   :height: 10cm  

   Layers tree panel.

Creating new vector layer from Custom forms (NGFP)
-----------------------------------------------------

.. versionadded:: 2.2

NGFP files can be generated using NextGIS FormBuilder. NGFP is a :term:`GeoJSON` file with additional information (JSON) which is packaged in zip archive and has .ngfp extension.

Perform the following steps to add NGFP file to NextGIS Mobile:

1. First tap on "Layers tree menue" (item 1 in :numref:`ngmobile_main_activity_pic_1`). Then tap on "Add geodata" (item 4 in :numref:`ngmobile_layer_tree_pic`) and select "Open local" (see :numref:`ngmobile_options_menu_new_layer_pic`) 

2. Select NGFP file from your mobile device storage (see :numref:`ngmobile_saved_files_on_the_drive_unit_pic`). E.g. tap on  "Structures.ngfp" to open the Structures layer.

.. figure:: _static/saved_files_on_the_drive_unit.png
   :name: ngmobile_saved_files_on_the_drive_unit_pic
   :align: center
   :height: 10cm
   
   Android local storage.

3. When the file is selected a layer settings dialog opens. Here you can specify a layer name (see :numref:`ngmobile_settind_layer_form_pic`): 

.. figure:: _static/settind_layer_form.png
   :name: ngmobile_settind_layer_form_pic
   :align: center
   :height: 10cm

   Layer settings dialog.
   
4. Pressing "Create" button starts data processing for creation of a new layer 

.. note::  
	In case of NGFP format data uploading the new layer will always be a vector type layer!

You can check if the new layer was created successfully in the layers tree panel. The newly created layer will show up in the layers tree (see :numref:`ngmobile_tree_layers_ngfp_pic`). The "Structures" layer is shown in orange rectangle.

.. figure:: _static/tree_layers_ngfp.png
   :name: ngmobile_tree_layers_ngfp_pic
   :align: center
   :height: 10cm  

   Layers tree panel.   

NGFP layers use custom (not standard) attributes form optimized for attributes viewing and editing. Custom form may contain special controls for editing, such as dropdowns, checkboxes or linked lists.

.. figure:: _static/non-standard_form.png
   :name: ngmobile_non-standard_form_pic
   :align: center
   :height: 10cm  
    
    Custom attributes form.

For more information about NGFP layer editing see :ref:`ngmobile_editing`.
