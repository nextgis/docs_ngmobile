.. sectionauthor:: Дмитрий Барышников <dmitry.baryshnikov@nextgis.ru><dmitry.baryshnikov@nextgis.ru>

.. tracks:

Tracks
======

NextGIS Mobile allows to record and display tracks. During the track recording points are storing in the internal database. When the track points are displaying within the session they are combining and displaying as a line on the map.

Record
------

To begin the record of track chose the command on the toolbar or in the menu (see :numref:`ngmobile_track_menu_pic` p. 1 p 2 accordingly). 

.. figure:: _static/ngmobile_track_menu.png
   :name: ngmobile_track_menu_pic
   :align: center
   :width: 5cm
   
   Track record command.

    The numbers indicate: 1 - track record button on the toolbar; 2 - track record menu item.

.. note::
	Commands moves to context menu if there is no enough space on the toolbar.

After choosing of command track record is beginning. Track record is performed free from app in the background mode. Status message is displaying in the status bar of operating system (see :numref:`ngmobile_status_track_pic`).

.. figure:: _static/ngmobile_status_track.png
   :name: ngmobile_status_track_pic
   :align: center
   :height: 5cm
 
 	Record track status.

 	The numbers indicate: 1 - name of track record session; 2 - button of finish track record; 3 - an app activation button of the track record process.

Recording track is displaying on the map immediately. Tracks points are grouped by days and sessions within the day. If the recording of track goes to next day, track will clash to two parts.  

Control
-------

Tracks are represented in a layers tree (see :numref:`ngmobile_layer_tree_pic`) as a group layer. The following operations can be performed over a group layer:

* on / off the visibility of the group layer (tracks);
* display of the tracks control window (see :numref:`ngmobile_settings_track_pic`).

.. figure:: _static/ngmobile_track_settings.png
   :name: ngmobile_settings_track_pic
   :align: center
   :height: 11cm
 
 	Track control window.

The numbers indicate: 1 - amount of selected tracks; 2 - button of all tracks selection (deselection); 4 - context menu; 5 - on / off display track button; 6 - track selection button; 7 - on / off of the tracks displaying menu item; 8 - delete selected tracks.

 The tracks control window contains a list of tracks. Tracks points are grouped by days and sessions within the day. None of the track will be highlighted when the tracks control window is open. You can only change the visibility of the individual track in this mode. Select the group of tracks to perform operations on them (see :numref:`ngmobile_settings_track_pic` Рї. 6). The window will look this way after you select at least one track :numref:`ngmobile_settings_track_pic`. In this case, the following operations can be performed on selected tracks:

 * on / off visibility;
 * delete.
