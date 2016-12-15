.. sectionauthor:: Dmitry Baryshnikov <dmitry.baryshnikov@nextgis.ru>

.. _ngmobile_share:

Exporting data
===============

Exporting data in GeoJSON
---------------------------

To export data from NextGIS Mobile vector layer, tap on "Layers tree menu" (item 1 in :numref:`ngmobile_main_activity_pic_1`). Then tap on the context menu button next to the layer name (item 5 in :numref:`ngmobile_layer_tree_pic`). This will pop up the context menu itms as shown in item 6 in :numref:`ngmobile_layer_tree_pic`. There you need to select "Share". Android standard Share dialog window with a list of available Share options will open as shown in :numref:`ngmobile_share_pic`.

.. figure:: _static/ngmobile_share.png
   :name: ngmobile_share_pic
   :align: center
   :height: 10cm
   
   Share dialog window.
   
After you select a share option, data in the selected layer will be recorded in :term:`GeoJSON` format (:term:`coordinate system` Web Mercator, EPSG:3857) and exported using the selected application. A name of the GeoJSON file corresponds to the name of the layer.

* You can send the file as attachment via your email App or Gmail.
* You can upload it to Google Drive, which may or may not be shared with your colleague.
* You can share it to another Android mobile via Bluetooth or SHAREit.
* You can even copy it on to your laptop via Bluetooth, if possible.

.. note::
   In a lot of Android versions to save a file on the device memory card you need a file manager app (for example, ES Explorer or similar).

Exporting attachments
-----------------------

Each feature in vector layer can have 1 or more photos attached to it. Photos are stored separately as image files and added to archive file with layer data during the export. For each feature a separate attachments folder is generated in the archive, the name of the folder correposnds to feature ID.

Example:

(4:10000002.jpg,10000000.jpg,10000001.jpg,10000003.jpg)

Explanation:

4 photos are attached to a feature. These 4 photos are stored in the folder which name correposnds to ID of this feature.

Exporting tracks in GPX
------------------------

To start exporting tracks first find "My Tracks" group layer in Layers tree. It is shown in the orange box. Then select the "Settings" item in a contextual menu as shown in :numref:`ngmobile_tree_layers_gpx_pic`. 

.. figure:: _static/tree_layers_gpx.png
   :name: ngmobile_tree_layers_gpx_pic
   :align: center
   :height: 10cm

   Layers tree.

Tracks control panel will open. If a few tracks have been recorded on same day, these tracks are grouped by sessions. If track recording continued for a few days, this track is split up into few parts corresponding to the number of days.

.. figure:: _static/tracks_list_gpx.png
   :name: ngmobile_tracks_list_gpx_pic
   :align: center
   :height: 10cm

   List of recorded tracks.

When you select the track by ticking on the Chekbox in front of it, buttons in Top toolbar will become active as shown in :numref:`ngmobile_layer_gpx_selected_pic` below

.. figure:: _static/layer_gpx_selected.png
   :name: ngmobile_layer_gpx_selected_pic
   :align: center
   :height: 10cm

   Toolbar for selected track.

When you tap to open contextual menu (see item 5 in :numref:`ngmobile_layer_gpx_selected_pic`), the associated menu items pop up as shown below in :numref:`ngmobile_layer_gpx_menu_pic`. 

.. figure:: _static/layer_gpx_menu.png
   :name: ngmobile_layer_gpx_menu_pic
   :align: center
   :height: 10cm   

   Tracks contextual menu.
   
* Here you can Show or Hide the selected track in the map screen. The starting point is shown in Green markere & the end point is shown in Red marker.
* You can delete the track (permanently).
* You can select all the tracks and perform above actions for all at a once.
