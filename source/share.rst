.. sectionauthor:: Dmitry Baryshnikov <dmitry.baryshnikov@nextgis.ru>

_ngmobile_share:

Exporting data
===============

Exporting data in GeoJSON
---------------------------

To export data from NextGIS Mobile vector layer open Layer tree and select "Share" in Layer contextual menu. Android standard Share dialog window with a list of available Share options (for example, by email, using cloud file storage, memory card, etc.) will open. Share dialog window is shown in :numref:`ngmobile_share_pic`.

.. figure:: _static/ngmobile_share.png
   :name: ngmobile_share_pic
   :align: center
   :height: 10cm
   
   Share dialog window.

After you select a share option data in the selected layer will be recorded in :term:`GeoJSON` format (:term:`coordinate system` Web Mercator, EPSG:3857) and exported using the selected application. A name of the GeoJSON file corresponds to the name of the layer.

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

To start exporting tracks first find "My Tracks" group layer in Layers tree. Then select the "Settings" item in a contextual menu  :numref:`ngmobile_tree_layers_gpx_pic`. 

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

Select tracks you want to export. Buttons in Top toolbar will become active. Open contextual menu and select "Share" item :numref:`ngmobile_tracks_list_and_menus_pic`. 

.. figure:: _static/tracks_list_and_menus.png
   :name: ngmobile_tracks_list_and_menus_pic
   :align: center
   :height: 10cm   

   Tracks control panel contextual menu.
