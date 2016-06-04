.. sectionauthor::  Наталья Барышникова <Nshelekhova@gmail.com>

.. _ngmobile_integration:

NextGIS Web integration
=======================

.. versionadded:: 2.2

.. only:: html
   
   You can find out more about the key features of NextGIS Web in subsection :ref:`ngweb_keyfeatures`.

   .. only:: latex

      You can find out more about the key features of NextGIS Web in subsection 'Key features of NextGIS Web <http://docs.nextgis.ru/docs_ngweb/source/general.html#ngweb-keyfeatures>`_.

.. _ngmobile_сreate_a_connection:

Create NextGIS Web connection 
-----------------------------

There are few ways to connect with NextGIS Web. Using **the first method** to connect NextGIS Web perform the following steps:

1. Open options menu (см. :numref:`ngmobile_main_activity_pic` p. 5). 
2. Select "New layer".
3. And choose the "NGW" item (see :numref:`ngmobile_add_ngw_layer_pic`) 

.. figure:: _static/add_layer1.png
   :name: ngmobile_add_ngw_layer_pic
   :align: center
   :height: 10cm
  
  	Adding NextGIS Web layer.

4. Select item "Add Account" (Add NextGIS Web account) and press the button (see :numref:`ngmobile_select_ngw_layer_pic`).

.. figure:: _static/select_layer.png
   :name: ngmobile_select_ngw_layer_pic
   :align: center
   :height: 10cm
   
   Adding NextGIS Web account.

5. Input NextGIS Web server :term:`URL`, your login/password and press "Login" (see :numref:`ngmobile_ngw_connection_settings_pic`).

.. figure:: _static/connection_settings.png
   :name: ngmobile_ngw_connection_settings_pic
   :align: center
   :height: 10cm

   Connection settings.

6. In case of successful connection, a window with established NextGIS Web account will open.

To connect to NextGIS Web using **the second method** perform following steps:

1. Open options menu (see :numref:`ngmobile_main_activity_pic` p. 5). 
	Select "Settings" item (see :numref:`ngmobile_settings2_pic`).

	.. figure:: _static/settings.png
   :name: ngmobile_settings2_pic
   :align: center
   :height: 10cm

   Options.

2. Choose item :menuselection:`NextGIS Web --> NextGIS Web settings (see :numref:`ngmobile_settings_ngw_pic`).  

.. figure:: _static/settings_NGW.png
   :name: ngmobile_settings_ngw_pic
   :align: center
   :height: 10cm
   
   Settings.

3. Select item "Add Account" in opened menu (see :numref:`ngmobile_add_entry_pic`).

.. figure:: _static/add_entry.png
   :name: ngmobile_add_entry_pic
   :align: center
   :height: 10cm

   Adding NextGIS Web account.

4. Input NextGIS Web server :term:`URL`, your login/password and press "Login" (see :numref:`ngmobile_ngw_connection_settings_pic`).

5. In case of successful connection, a window with created NextGIS Web account will open.

.. note::
	In the dialog box of input NextGIS Web connections parameters enter login/password without spaces! A lot of smartphones and tablets keyboards make autosubstitution of text and when you insert copied text from the clipboard a space adds to the end of the text in the input field (login/password). The end-result text with a space is perceived by NextGIS Web like another login or password, it leads to connection’s fail.

Deleting NextGIS Web account
----------------------------

You can delete the NextGIS Web account in several ways. When you are using the **first method** to delete NextGIS Web account perform the following steps:
1. Open options menu (see :numref:`ngmobile_main_activity_pic` p. 5). 
2. Then open "Settings" (see :numref:`ngmobile_settings2_pic`).
3. Select item "NextGIS Web" (see :numref:`ngmobile_settings_ngw_pic`). 
4. Choose created before NextGIS Web account (see :numref:`ngmobile_select_ngw_layer_pic`).
5. Select "Delete account" item (see :numref:`ngmobile_remove_account_pic`).

.. figure:: _static/remove_account.png
   :name: ngmobile_remove_account_pic
   :align: center
   :height: 10cm
    
    Deleting NextGIS Web account.

6. Delete selected NextGIS Web account.
7. If account will be deleted successfully window of app will open without the NextGIS Web account created before.

To delete NextGIS Web account using  **second method** perform the following steps:

1. Open "Settings" of your Android device.
2. Scroll to Accounts options.
3. Select "NextGIS Web" account (see :numref:`ngmobile_accounts_in_os_pic`).

.. figure:: _static/accounts_in_os.png
   :name: ngmobile_accounts_in_os_pic
   :align: center
   :height: 10cm
   
   Selecting NextGIS Web account in Android settings.

4. Select created before the NextGIS Web account and press the button "Delete account" in the bottom right corner of screen. (see :numref:`ngmobile_remove_account_in_os_pic`).

.. figure:: _static/remove_account_in_os.png
   :name: ngmobile_remove_account_in_os_pic
   :align: center
   :height: 10cm
   
   Deliting NextGIS Web account through Android settings.

5. Delete selected NextGIS Web account.
6. If account will be deleted successfully window of app will open without the NextGIS Web account created before.

4.9.3. Adding the layer (vector or raster) from NextGIS Web
----------------------------------------------------
To add the layer (vector or raster) from NextGIS Web perform the following steps:

1. Open options menu (see :numref:`ngmobile_main_activity_pic` p. 5). 
2. Select "New layer" item.
3. Choose the "Add from NGW" item (see :numref:`ngmobile_add_ngw_layer_pic`).
4. Select account in the list (see :numref:`ngmobile_select_ngw_layer_pic`). 
Read more about how to create an account in chapter ":ref:`ngmobile_сreate_a_connection`".

5. There is a list of internal resources and layers NextGIS Web (vector and rasters) of selected account in opened window (see :numref:`ngmobile_list_of_files_pic`).

.. figure:: _static/list_of_files.png
   :name: ngmobile_list_of_files_pic
   :align: center
   :height: 10cm
   
   List of resources and layers of NextGIS Web.

6. Select the desired group of NextGIS Web resources and notice required NextGIS Web layer (vector or raster) by affixing marks and choosing of the "Select" menu item. (see :numref:`ngmobile_file_selection_pic`).

.. figure:: _static/file_selection.png
   :name: ngmobile_file_selection_pic
   :align: center
   :height: 5.85cm

   Selecting required layer in the NextGIS Web resources group.

.. note::
	It should be noted that if it is necessary to select multiple NextGIS Web layers (vector and/or raster) in the different resources groups of one account, the affixed mark of selected layer will be saved during moves from one resources group to another.

7. There are items "Cancel" and "Hide" in the opened window of selected layer processing (see :numref:`ngmobile_processing_layer_pic`).

.. figure:: _static/processing_layer.png
   :name: ngmobile_processing_layer_pic
   :align: center
   :height: 10cm

   Processing the layer.

Select the "Cancel" item menu if you need to stop the processing procedure of NextGIS Web layer. To prevent blocking of the interface and for further work with the NextGIS Mobile select item menu "Hide". In the result of this selection the NextGIS Web layer processing bar will be moved to the status bar (see :numref:`ngmobile_download_status_pic`).

.. figure:: _static/download_status.png
   :name: ngmobile_download_status_pic
   :align: center
   :height: 10cm

   Status bar.

If it is necessary to finish the process of NextGIS Web layer is going (which is moved to the status bar) you must do the following: tap the screen by your thumb and forefinger and split them apart sliding by screen. As a result of this action the processing indicator of NextGIS Web layer will be moved to the status bar and the button "Stop" will appear. If you press the button "Stop" the process of processing will be finished. As a result this actions the selected NextGIS Web layers (vector and/or raster) will be added on the map and appear in the layers tree on the top. 
Data will not be lost if there were previously created on the map NextGIS Web points and/or lines and it will be in the layers tree in a certain order.
You can configure the viewing of map composition, control the visibility and order of layers in  the layers tree after processing and the creation of new NextGIS Web layers on the map (raster and/or vector).

Setting up synchronization of vector layer with NextGIS Web
-----------------------------------------------------------

Use synchronization for process of operational geodata revisions exchange and providing identity of selected information between the PC and user's mobile device. Perform the following steps for synchronize vector layer with NextGIS Web:

1. Open options menu.
2. Choose "Settings" menu item (see :numref:`ngmobile_settings2_pic`).
3. In the "Settings" menu select "NextGIS Web/ NextGIS Web settings" (see :numref:`ngmobile_settings_ngw_one_pic`).  

.. figure:: _static/settings_NGW.png
   :name: ngmobile_settings_ngw_one_pic
   :align: center
   :height: 10cm
   
   The settings.

4. From available list select the desired account (see :numref:`ngmobile_add_entry_one_pic`).

.. figure:: _static/add_entry.png
   :name: ngmobile_add_entry_one_pic
   :align: center
   :height: 10cm
   
   Accounts list.

5. There are next items in the opened window: (see :numref:`ngmobile_conntction_properties_window_pic`):

	- synchronization/ automatic synchronization with checkbox; 
	- synchronization of specific layer with NextGIS Web;
	- synchronization interval (can be changed from 5 minutes to 2 hours).

	.. figure:: _static/conntction_properties_window.png
   :name: ngmobile_conntction_properties_window_pic
   :align: center
   :height: 10cm
 
 	Connection settings.

The icon with the circled arrows will appear near the layer symbol after selecting the layer and affixing the mark about permission of process synchronization with NextGIS Web. The same icon will appear in the layers tree opposite of synced layer (see :numref:`ngmobile_layers_tree_int_pic`):

.. figure:: _static/layers_tree_int.png
   :name: ngmobile_layers_tree_int_pic
   :align: center
   :height: 10cm

   Layers tree.
