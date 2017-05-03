.. sectionauthor:: Dmitry Baryshnikov <dmitry.baryshnikov@nextgis.ru>, Abhay Kulkarni <praxisnfp@gmail.com>

.. _ngmobile_share:

Exporting data
===============

.. _ngmobile_export_vector:

Exporting data in GeoJSON
---------------------------

To export data from NextGIS Mobile vector layer open Layers tree panel (item 1 in :numref:`ngmobile_main_activity_pic_1`). Then tap on the contextual menu icon next to the layer name (item 5 in :numref:`ngmobile_layer_tree_pic`). This will open the contextual menu items as shown in item 6 in :numref:`ngmobile_layer_tree_pic`. There you need to select "Share". 

Android standard Share dialogue window with a list of available Share options will open as shown in :numref:`ngmobile_share_pic`.

.. figure:: _static/ngmobile_share.png
   :name: ngmobile_share_pic
   :align: center
   :height: 10cm
   
   Share dialogue window.
   
After you select a share option, data in the selected layer will be recorded in :term:`GeoJSON` format (:term:`coordinate system` Web Mercator, EPSG:3857) and exported via the selected application. The name of GeoJSON file will be the same as the name of the exported layer.

Some of the share options (availability is dependant on the apps installed on your device):
* You can send the file as an attachment via Gmail or different Email app.
* You can upload the file to Google Drive/Dropbox/other cloud service and then share it with your colleagues.
* You can send the file to another device via Bluetooth or SHAREit.
* You can save the file on a memory card.

.. warning::
   In many Android versions to save a file on the device memory card you need a file manager app (for example, ES Explorer or similar).

Exporting attachments
-----------------------

Each feature in vector layer can have 1 or more photos attached to it. Photos are stored separately as image files and added to archive file with layer data during the export. For each feature a separate attachments folder is generated in the archive, the name of the folder corresponds to feature ID.

Example:

(4:10000002.jpg,10000000.jpg,10000001.jpg,10000003.jpg)

Explanation:

4 photos are attached to a feature. These 4 photos are stored in the folder which name is similar to the feature ID.

.. _ngmobile_export_GPX:

Exporting tracks in GPX
------------------------

To start exporting tracks first find "My Tracks" group in Layers tree panel. Then tap on contextual menu button as shown in :numref:`ngmobile_tree_layers_gpx_pic` and select "List".

.. figure:: _static/tree_layers_gpx.png
   :name: ngmobile_tree_layers_gpx_pic
   :align: center
   :height: 10cm

   "My tracks" in Layers tree panel.

This will open a list of recorded tracks as shown in :numref:`ngmobile_tracks_list_gpx_pic`.

Select a track you want to export by ticking the corresponding checkbox, and buttons in Top toolbar will become active as shown in  :numref:`ngmobile_layer_gpx_selected_pic`.

To export the track, tap on Share button (see item 4 in :numref:`ngmobile_layer_gpx_selected_pic`). It will open the same Share dialogue window as shown in :numref:`ngmobile_share_pic` above.

After you select a share option, data in the selected track will be recorded in GPX format and exported via the selected application.
