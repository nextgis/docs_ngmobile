.. sectionauthor:: Дмитрий Барышников <dmitry.baryshnikov@nextgis.ru>

.. _ngmobile_gui:

User interface (UI)
==========================

There are 3 major elements of NextGIS Mobile UI:

* Main screen
* Layers tree panel
* Settings dialog

UI is designed in accordance with `Google Material design <http://www.google.com/design/spec/material-design/introduction.html>`_ guidelines.

.. _ngmobile_main_activity:

Main screen
------------

Main screen is shown on :numref:`ngmobile_main_activity_pic`.

.. figure:: _static/ngmobile_mainscreen.png
   :name: ngmobile_main_activity_pic
   :align: center
   :height: 11cm
   
   Main screen.

   The numbers indicate: 1 - Layers tree panel icon; 2 - Application title; 3 – "Add geodata" button; 4 - "Show my location" button; 5 - Contextual menu icon; 6 - Map screen; 7 - Main actions button; 8 - Status bar.

The number of buttons in top toolbar depends on your device screen size. If the buttons don't fit into the toolbar they are moved to the contextual menu (item 5 in :numref:`ngmobile_main_activity_pic`).

**Top toolbar** contains the following buttons:

* Add :term:`geodata`
* Show my location
* Start new track
* Settings
* About

"Add geodata" button (item 3 in :numref:`ngmobile_main_activity_pic`) allows you to select the data source using the following menu:

* Open local
* Add web
* Add from NGW

By using "Open local" menu item you can upload :term:`geodata` from SD card or cloud storage, in one of the following formats:

* :term:`GeoJSON` file;
* ZIP file with cached tiles;
* *.ngfp format.

More information about geodata upload can be found in ":ref:`ngmobile_load_geodata`" section.

**Map screen** (item 6 in :numref:`ngmobile_main_activity_pic`) is a set of raster and vector layers. Hierarchy and visibility of layers can be configured in the layers tree panel (see :ref:`ngmobile_layer_tree`).

Long-press on vector layer geometry switches map screen into Selection mode (see :numref:`ngmobile_selectmode_pic`).

.. figure:: _static/ngmobile_selectmode.png
   :name: ngmobile_selectmode_pic
   :align: center
   :height: 11cm

   Map screen in Selection mode.

   The numbers indicate: 1 - Selected geometry; 2 - "View attributes" button; 3 - "Delete geometry" button; 4 - "Edit geometry" button; 5 - Cancel button.
   
If Status bar was active before switching to Selection mode, it will be hidden and replaced by Bottom toolbar with the following buttons:

* Cancel
* Edit selected geometry (see :ref:`ngmobile_editing`)
* Delete selected geometry
* View attributes of selected geometry.

Attributes are displayed in a separate panel. Panel can be opened in full-screen mode or be placed on the right side of screen, depending on your device screen size (in the latter case, on the left side a map with a selected and highlighted geometry is displayed). Attributes panel is shown on :numref:`ngmobile_attributes_pic`.

.. figure:: _static/ngmobile_attributes.png
   :name: ngmobile_attributes_pic
   :align: center
   :height: 10cm
   
   Attributes panel.

There are the following buttons at the bottom of the Attributes panel: "Cancel" and "Switch between entries" (If Status bar was active before opening Attributes panel, it will be hidden and replaced by these buttons).

**Status bar** can be shown at the bottom of the Main screen (if it is activated in the Settings). Status bar shows:

* Device coordinates (latitude and longitude);
* Positioning signal source (mobile networks/Wi-Fi or satellite) and number of captured satellites (if positioning is carried out with help of :term:`GPS`/:term:`GLONASS`);
* Device altitude (meters);
* Device speed (kmph)

Depending on the size of the screen Status bar can occupy one or two rows.

.. _ngmobile_layer_tree:

Layers tree
------------

Layers tree panel is designed to show the content of a map and to control the visibility and hierarchy of map layers. Additional operations with layers are available from a separate layer contextual menu. Layers tree panel is shown on: numref: `ngmobile_layer_tree_pic`.

.. figure:: _static/ngmobile_layertree.png
   :name: ngmobile_layer_tree_pic
   :align: center
   :height: 11cm
   
   Layers tree panel.

   The numbers indicate: 1 - Layer type; 2 - Layer name; 3 - Layer visibility button; 4 - Layer contextual menu icon; 5 - Layer contextual menu.

To change the hierarchy of map layers long-press the layer which is to be moved up or down. Layers tree panel will switch to Edit mode. Keep pressing and move the selected layer to its new position.

For turning  layer visibility on/off press Layer visibility button (item 3 in :numref:`ngmobile_layer_tree_pic`).

Layer contextual menu depends on layer's type. Vector layer contextual menu contains the following items:

* Zoom to extent
* Share
* Delete
* Settings

By pressing "Delete" you not only remove layer from the map but also erase all its data from the memory card.

.. _ngmobile_settings:

Settings dialog
-------------------

Depending on the screen size Settings dialog can fit into one or two panels. Settings dialog is shown on :numref:`ngmobile_settings_pic` (one panel mode).

.. figure:: _static/ngmobile_settings.png
   :name: ngmobile_settings_pic
   :align: center
   :height: 10cm
   
   Settings.

There are following Settings on the main panel:

* General
* Map
* Location
* My tracks
* NextGIS Web

"Map" settings allow to change basic settings of the map (see :numref:`ngmobile_settings_map_pic`).

.. figure:: _static/ngmobile_settings1.png
   :name: ngmobile_settings_map_pic
   :align: center
   :height: 10cm
   
   Map settings.

Map settings include:

* Show/hide Status bar
* The way current location displays (show position and accuracy, show only position, do not show position)
* Show mini compass
* Do not turn off the screen when map displays - works only on the map screen
* Show/hide zoom control buttons
* Coordinates format (for coordinates in Status bar and other dialogs and screens)
* Map background (light, dark, neutral)
* Map path (here you can specify a path where map and layers data will be stored)

.. note::
	For devices with several SD cards and Android 4.4 and higher, map path not on the main SD card can only be specified in the application home directory and its subdirectories (for example: Android/data/com.nextgis.mobile). This is also true for some devices without root access. Read-only folders won't show up in path selection dialog.

"Location" settings contain location settings (see :numref:`ngmobile_settings_place_pic`).

.. figure:: _static/ngmobile_settings2.png
   :name: ngmobile_settings_place_pic
   :align: center
   :height: 10cm
   
   Location settings.

Location settings include:

* Coordinate source (mobile networks/Wi-Fi + :term:`GPS` or only GPS)
* Minimum update time
* Minimum update distance
* Count of GPS fixes

"Tracks" settings are similar to the location settings, but they are applied only for track recording.

.. Note::

   If you set value of the minimum update distance at more than 5 m, the operating system will start to smooth the track (remove outliers).
