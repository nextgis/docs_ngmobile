.. sectionauthor:: Дмитрий Барышников <dmitry.baryshnikov@nextgis.ru>

.. _ngmobile_gui:

User interface
==========================

There are 3 major elements in application interface:

* Main window;
* Sliding panel for layers tree;
* Settings.

Application interface is designed in accordance with `Google Material design <http://www.google.com/design/spec/material-design/introduction.html>`_ guidelines.

.. _ngmobile_main_activity:

Main Window
------------

Main window is shown on :numref:`ngmobile_main_activity_pic`.

.. figure:: _static/ngmobile_mainscreen.png
   :name: ngmobile_main_activity_pic
   :align: center
   :height: 11cm
   
   Main Window.

   The numbers indicate: 1 - open sliding panel for layers tree; 2 - application title; 3 – add geodata; 4 - my position; 5 - options; 6 - map screen; 7 - list of main operations; 8 - status bar.

The number of buttons on the top toolbar depends on the size of screen. If the buttons do not fit on the toolbar, they will be moved to the menu (see :numref:`ngmobile_main_activity_pic` p. 5).

Toolbar has the following tools:

* Start new track
* Add :term:`geodata`;
* Settings;
* About.

Map (see :numref:`ngmobile_main_activity_pic` p. 6) is a set of raster and vector layers. Order and visibility of layers can be configured in the layers tree (see :ref:`ngmobile_layer_tree`).

Button "add geodata" (see :numref:`ngmobile_main_activity_pic` p. 3) opens the next menu:

* Open local
* Add web
* Add from NGW

Selecting "local" menu will open dialog for choosing path to :term:`geodata` from SD card or from cloud storage as well. NextGIS allows to upload the following geodata formats:

* :term:`GeoJSON` file;
* ZIP file with cached tiles;
* *.ngfp format.

More information about geodata loading can be found in chapter ":ref:`ngmobile_load_geodata`".

While holding finger on the geometry of vector layer the map screen switches into action mode selection (see :numref:`ngmobile_selectmode_pic`).

.. figure:: _static/ngmobile_selectmode.png
   :name: ngmobile_selectmode_pic
   :align: center
   :height: 11cm

   Map screen in selection mode.

   The numbers indicate: 1 - selected geometry; 2 - attribute view; 3 - delete geometry; 4 - edit geometry; 5 - finish selection mode.
   
If status bar was open before selection, it will be hidden and replaced by bottom toolbar with the following buttons:

* Cancel;
* Start editing of selected geometry (see :ref:`ngmobile_editing`);
* Remove selected geometry;
* Show attributes of selected geometry.

Attributes are displayed in a separate panel by choosing show attributes mode. Panel can be opened in fullscreen mode or be placed on the right side of screen, depending on the size of the screen of your device (in the left side displays a map with highlighted geometry which is currently selected). Attributes panel is shown on :numref:`ngmobile_attributes_pic`.

.. figure:: _static/ngmobile_attributes.png
   :name: ngmobile_attributes_pic
   :align: center
   :height: 10cm
   
   Attributes panel.

There are the following buttons at the bottom of the attributes panel: exit attributes display and switch between entries (if the information bar was active, it is hidden).

At the bottom of the screen status bar can be placed (when the appropriate option in the settings is on). Status bar shows:

* Coordinates (latitude and longitude);
* Positioning signal source (mobile networks/Wi-Fi or satellite) and number of captured satellites (if positioning is carried out with help of :term:`GPS`/:term:`GLONASS`);
* Altitude (meters);
* Speed (km/h)

Depending on the size of the screen the status bar can occupy one or two rows.

.. _ngmobile_layer_tree:

Layers tree
-----------

Layers tree is designed to show the content of a map and to control the visibility and order of layers. Additional operations over the layers are placed into a separate layer menu. Layers tree is shown on: numref: `ngmobile_layer_tree_pic`.

.. figure:: _static/ngmobile_layertree.png
   :name: ngmobile_layer_tree_pic
   :align: center
   :height: 11cm
   
   Layers tree of map.

   The numbers indicate: 1 - icon of the layer; 2 - name of the layer; 3 - visibility switch 4 - button of the context layer menu display; 5 - context layer menu.

To change the order of layers hold your finger on the layer which has to be moved. After that a list will switch to the change layers order mode. Then, holding finger on screen, just move the layer to the new position.

For turning on/turning off layer visibility push on the corresponding icon (see :numref:`ngmobile_layer_tree_pic`, p. 3).

The context layer menu depends on layer's type. Vector layer menu has the following items:

* Zoom to extent
* Share
* Delete
* Settings

If you select "Delete" layer would be removed from the map, and all its data would be erased from the memory card.

.. _ngmobile_settings:

Settings
--------

Depending on the screen size the settings window can show one or two panels. Settings window is shown on :numref:`ngmobile_settings_pic` (one panel mode).

.. figure:: _static/ngmobile_settings.png
   :name: ngmobile_settings_pic
   :align: center
   :height: 10cm
   
   Settings.

There are following settings blocks on the main panel:

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

Map settings are:

* Show/hide status bar;
* The way current location displays - show position and accuracy, only position, do not show position;
* Show mini compass;
* Do not turn off the screen when map displays - works only in the map window;
* Show/hide zoom control buttons;
* Coordinates format - actual for coordinates in status bar and other dialogs and windows;
* Map background;
* Map path - here you can specify a path where map and layers data will be stored.

.. note::
	In the case of devices with several SD cards and operating system Android 4.4 (KitKat) and above, the path to the map not on the main SD card may only be specified in the application home directory and its subdirectories (for example: Android/data/com.nextgis.mobile). This is also true for some devices without root access.

Read-only folders won't show up in selection dialog.

"Location" settings block contains location settings (see :numref:`ngmobile_settings_place_pic`).

.. figure:: _static/ngmobile_settings2.png
   :name: ngmobile_settings_place_pic
   :align: center
   :height: 10cm
   
   Location settings.

Location settings are:

* Coordinate source (mobile networks/Wi-Fi + :term:`GPS` or only GPS);
* Minimum update time
* Minimum update distance
* Count of GPS fixes

Tracks settings are similar to the location settings, but they only influence track recording.

.. Note::

   If you put the value of the minimum update distance more than 5 m, the operating system will starts to smooth the track (removes outliers).
