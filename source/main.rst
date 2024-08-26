.. sectionauthor:: Dmitry Baryshnikov <dmitry.baryshnikov@nextgis.ru>, Abhay Kulkarni <praxisnfp@gmail.com>

.. _ngmobile_gui:

User interface (UI)
==========================

There are 4 major elements of NextGIS Mobile UI:

* Main screen
* Layers tree panel
* Features table
* Settings dialogue

UI is designed in accordance with `Google Material design <http://www.google.com/design/spec/material-design/introduction.html>`_ guidelines.

.. _ngmobile_main_activity:

Main screen
------------

Main screen is shown on :numref:`ngmobile_main_activity_pic_1`.

.. figure:: _static/ngmobile_mainscreen_1.png
   :name: ngmobile_main_activity_pic_1
   :align: center
   :width: 10cm
   
   Main screen

   The numbers indicate: 1 - Layers tree panel icon; 2 - Application title; 3 – "Show my location" button; 4 - "Load/Refresh geodata" button; 5 - Contextual menu icon; 6 - Measuring button; 7 - Map screen; 8 - Main actions button; 9 - Status info panel.

The number of buttons in top toolbar depends on your device screen size. If the buttons don't fit into the toolbar they are moved to the contextual menu (item 5 in :numref:`ngmobile_main_activity_pic_1`).

**Top toolbar** contains the following buttons:

* Show my location
* Load or refresh geodata
* Start new track
* Settings
* Help

**Status info panel** (item 9 in :numref:`ngmobile_main_activity_pic_1`) can be shown at the bottom of the Main screen (if it is activated in the Settings - Map - Show status info panel). Status info panel shows (if there is the fixed location):

* Device coordinates (latitude and longitude);
* Positioning signal source (mobile networks/Wi-Fi or satellite) and number of captured satellites (if positioning is carried out with help of :term:`GPS`/:term:`GLONASS`);
* Device altitude (meters);
* Device speed (kmph)

Depending on the size of the screen Status info panel can occupy one or two rows.

A map (item 7 in :numref:`ngmobile_main_activity_pic_1`) is a set of raster and vector layers. 
The order and the visibility of layers are under control of layers tree (:ref:`ngmobile_layer_tree`).


After a long hold of your finger on the vector layer's geometry the map window 
turns to the select mode. 

.. _ngmobile_layer_tree:

Layers tree
------------

Layers tree panel is designed to display the content of a map and to control visibility and hierarchy of map layers. Additional operations with layers are available from a separate layer contextual menu. Layers tree panel is shown on :numref:`ngmobile_layer_tree_pic`.

.. figure:: _static/ngmobile_layer_tree_eng_new.png
   :name: ngmobile_layer_tree_pic
   :align: center
   :width: 10cm
   
   Layers tree panel

   The numbers indicate: 1 - Layer type; 2 - Layer name; 3 - Layer visibility button; 4 - Add geodata; 5 - Layer contextual menu icon; 6 - Layer contextual menu items.
   
To change the hierarchy of map layers long-press the layer which is to be moved up or down. Layers tree panel will switch to Edit mode. Keep pressing and move the selected layer to its new position.

For turning layer visibility on/off tap on Layer visibility button (item 3 in :numref:`ngmobile_layer_tree_pic`).

"Add geodata" button (item 4 in :numref:`ngmobile_layer_tree_pic`) allows you to create vector layers and import vector and raster layers from Android local storage, `QuickMapServices catalog <https://qms.nextgis.com/>`_, `nextgis.com <https://my.nextgis.com/signup/?next=/webgis/>`_ or `NextGIS Web <http://nextgis.com/nextgis-web/>`_. This button contains the next menu (:numref:`options_menu_new_layer`):

* Create layer;
* Open local;
* Add geoservice;
* Add from NextGIS.

.. figure:: _static/options_menu_new_layer.png
   :name: options_menu_new_layer
   :align: center
   :width: 10cm
   
   Add geodata dialogue

By using "Open local" menu item you can upload :term:`geodata` from local storage in one of the following formats:

* :term:`GeoJSON` file;
* ZIP file with cached tiles;
* *.ngrc file
* *.ngfp file.

More information about geodata upload can be found in ":ref:`ngmobile_load_geodata`" section.

Layer contextual menu depends on layer's type (whether it is vector or raster layer). When you tap the Contextual menu button (item 5 in :numref:`ngmobile_layer_tree_pic`) contextual menu items pop up as shown by item 6 in :numref:`ngmobile_layer_tree_pic`

* Zoom to extent
* Features table
* Share
* Send to NextGIS
* Edit
* Delete
* Settings

.. warning::
   By pressing "Delete" you not only remove layer from the map but also erase all its data from the local storage.

.. _ngmobile_attributes_table:

Features table
-----------------

Features table is designed to show and manage the contents of each vector layer in table format.

To open Features table activate Layers tree panel and tap on the Contextual menu button next to the vector layer name (item 5 in :numref:`ngmobile_layer_tree_pic`). This will pop up the contextual menu items as shown by item 6 in :numref:`ngmobile_layer_tree_pic`. There you need to select "Features table". Depending on the screen size the panel could occupy the whole screen or just the right side (in this case there is a map with a highlighted geometry of the current attributes on the left side). 

Features table opens as shown in :numref:`ngmobile_attribute_table_pic` below.

.. figure:: _static/attribute_table_new.png
   :name: ngmobile_attribute_table_pic
   :align: center
   :width: 10cm
   
   Features Table

If you tap any record (row) in the table, the Features table toolbar appears at the bottom of the screen. This toolbar allows to manage features as shown below in :numref:`ngmobile_attribute_table_toolbar_pic`.

.. figure:: _static/attribute_table_toolbar_new.png
   :name: ngmobile_attribute_table_toolbar_pic
   :align: center
   :width: 10cm
   
   Features table toolbar
   
   The numbers indicate: 1 - Close Features table; 2 - Layer name; 3 - Features attributes;  4 - Close toolbar; 5 - Selected feature ID; 6 - Show selected feature on the map; 7 - Delete selected feature; 8 - Open Features table editing form.
   
You can open the standard Features table editing form as shown in :numref:`ngmobile_input_form_attributes_pic` by selecting "Open Features table editing form" (see item 8 in :numref:`ngmobile_attribute_table_toolbar_pic`)  
   
.. warning::
   If you tap on "Delete" button (see item 7 in :numref:`ngmobile_attribute_table_toolbar_pic`), the system will delete the selected feature immediately. You will be able to undo the removal, but if undo action is not applied in 5 seconds after removal, the feature gets deleted permanently.   

.. _ngmobile_settings:

Settings dialogue
------------------

Depending on the screen size Settings dialogue can fit into one or two panels. Settings dialogue is shown on :numref:`ngmobile_settings_pic` (one panel mode).

.. figure:: _static/ngmobile_settings_eng_new.png
   :name: ngmobile_settings_pic
   :align: center
   :width: 8cm
   
   Settings

There are following Settings on the main panel:

* General
* Map
* Location
* My tracks
* Web GIS
* Account

.. _ngmobile_settings_gen:

General
~~~~~~~~~~~

"General" settings allow to change basic settings of the map (see :numref:`ngmobile_settings_general_pic`).

.. figure:: _static/ngmobile_settings3en.png
   :name: ngmobile_settings_general_pic
   :align: center
   :width: 10cm
   
   General settings
   
Here you can select the theme (Light or Dark) and tune up compass settings.

"Map" settings allow to change basic settings of the map (see :numref:`ngmobile_settings_map_pic`).

.. figure:: _static/ngmobile_settings1.png
   :name: ngmobile_settings_map_pic
   :align: center
   :width: 10cm
   
   Map settings

.. _ngmobile_settings_map:

Map
~~~~~

Map settings include:

* Show/hide Status info panel
* The way current location displays (show current location, show marker, how marker & accuracy radius)
* Show mini compass
* Do not turn off the screen when map displays - works only on the map screen
* Show/hide zoom control buttons
* Show scale ruler
* Show measuring button
* Coordinates format (for coordinates in Status bar and other dialogs and screens)
* Decimal places
* Map background (light, dark, neutral)
* Map path (here you can specify a path where map and layers data will be stored)

.. note::
	For devices with several SD cards and Android 4.4 and higher, map path not on the main SD card can only be specified in the application home directory and its subdirectories (for example: Android/data/com.nextgis.mobile). This is also true for some devices without root access. Read-only folders won't show up in path selection dialog.

.. _ngmobile_settings_loc:

Location
~~~~~~~~

"Location" settings offer a few location specific settings (see :numref:`ngmobile_settings_place_pic`).

.. figure:: _static/ngmobile_settings2.png
   :name: ngmobile_settings_place_pic
   :align: center
   :width: 10cm
   
   Location settings

Location settings include:

* Coordinate source (mobile networks/Wi-Fi + :term:`GPS`, Other networks or only GPS)
* Minimum update time
* Minimum update distance
* Count of GPS fixes

.. _ngmobile_settings_tracks:

My tracks
~~~~~~~~~~

"Tracks" settings are similar to the location settings, but they are applied only for track recording.

Check "Send location to server" if you want to view tracks on a Web Map or save them to a vector layer. In this settings page you can also check your UID (you'll need it to create a tracker in Web GIS). `More about tracking <https://docs.nextgis.com/docs_ngcom/source/tracking.html>`_.

.. figure:: _static/Mobile_send_to_server_en.png
   :name: my_tracks_settings_pic
   :align: center
   :width: 10cm

   My tracks settings

.. note::
   If you set value of the minimum update distance at more than 5 m, the operating system will start to smooth the track (remove outliers).

.. _ngmobile_useful_facilities:

Useful features
-----------------

From the Main screen itself you can access a couple of features useful in the field.

.. _ngmobile_show_my_location:

Show my location
^^^^^^^^^^^^^^^^

To know your current location, just tap on the "Show my location" button (see item 3 in :numref:`ngmobile_main_activity_pic_1` above). This will show your current location on the map screen with a marker. If your Status info panel (see item 9 in :numref:`ngmobile_main_activity_pic_1` above) is switched on via appropriate Map settings (see :numref:`ngmobile_settings_map_pic`) you'll also be able to view the relevant information there.

.. note::
   Your "Location" settings must be switched ON in your Android mobile settings.
   
Measure distance and area
^^^^^^^^^^^^^^^^^^^^^^^^^^

It is possible to measure the distance between two points directly on the map screen. Just tap on the Measuring button on Map screen (see item 6 in :numref:`ngmobile_main_activity_pic_1` above). Tap on your starting point (a new point in Edit mode will appear on the screen). Then tap on your finishing point (a second point in Edit mode and line between the points will appear on the screen). The distance between two points will be shown in Top toolbar. See :numref:`ngmobile_measure_distance_pic` below for illustration.

.. figure:: _static/measure_distance.png
   :name: ngmobile_measure_distance_pic
   :align: center
   :width: 10cm
   
   Measure distance

   The numbers indicate: 1 - Layers tree panel icon; 2 - Measured distance; 3 - “Show my location” button; 4 - “Load/Refresh geodata” button; 5 - Contextual menu icon; 6 - Zoom controls; 7 - Exit Measuring mode.

Position of any point may be edited by tapping on it and dragging it to the correct location.

You can add additional points to measure distance of angled lines and smooth curves, as well as measure areas of the formed polygons. 

To exit Measure mode tap the blue tick button in the corner of the screen (see item 7 in :numref:`ngmobile_measure_distance_pic`).

.. note::
   To use this feature "Show measuring button" checkbox must be switched ON in Map settings (see :numref:`ngmobile_settings_map_pic`).

.. _ngmobile_view_info:

How to view feature information
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

Make a short tap on a feature and a tool bar will appear at the bottom on the screen. The only active option will be "info" (i in a circle). Press it to view the attributes and attachments of the feature.
