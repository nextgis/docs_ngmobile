.. _ngmobile_integration:

Integration with NextGIS Web 
==============================

.. only:: html
   
   You can learn more about the main features of Web GIS in :ref:`Web GIS <ngcom_description>`. 


.. only:: latex

   You can learn more about the main features of Web GIS 
   in `Web GIS: Description and Main Features <https://docs.nextgis.com/docs_ngcom/source/description.html#ngcom-description>`_.

NextGIS Mobile can be connected to a Web GIS created on the NextGIS Web platform. This integration allows to exchange data with a Web GIS: upload local layers to the server, download data from the server, edit the data, view tracks recorded with the app on a Web Map.

To add a connection to a Web GIS, you need to be `logged in <https://docs.nextgis.com/docs_ngmobile/source/auth.html>`_.

If the NextGIS ID already has a Web GIS associated with it, it will be automatically added to the app. All the Web GIS where the user is a `team member <https://docs.nextgis.com/docs_ngcom/source/teams.html>`_ will also be added.

If you don't have a Web GIS yet, `create it <https://docs.nextgis.com/docs_ngcom/source/create_webgis.html>`_ from your account.

You can add more connections to `cloud-based Web GIS <https://docs.nextgis.com/docs_ngmobile/source/ngw_integration.html#ngmobile-create-a-connection>`_ as well as `on-premise Web GIS  <https://docs.nextgis.com/docs_ngmobile/source/ngw_integration.html#ngm-create-connection-onp>`_.

You can `edit <https://docs.nextgis.com/docs_ngmobile/source/ngw_integration.html#ngmobile-change-account>`_ or `delete <https://docs.nextgis.com/docs_ngmobile/source/ngw_integration.html#ngmobile-delete-account>`_ a Web GIS connection.




.. _ngmobile_create_a_connection_to_webgis:

Add Web GIS connection
----------------------

There are two ways to connect your NextGIS Mobile app to a Web GIS. 

**Via layer tree**

1. Open Layers tree panel (item 1 in :numref:`ngmobile_main_activity_pic_1`). 
2. Then tap on "Add geodata" button (item 4 in :numref:`ngmobile_layer_tree_pic`).
3. Select “Add from Web GIS”. 

.. figure:: _static/ngm_layer_tree_add_from_wg_en.png
   :name: ngmobile_the_menu_button_add_pic
   :align: center
   :width: 10cm
  
   Add geodata dialog

4. In the opened dialog select “Add Web GIS”.

.. figure:: _static/ngm_add_webgis_en.png
   :name: ngm_add_webgis_pic
   :align: center
   :width: 10cm
   
   Web GIS dialog
   
5. On the next screen enter the Web GIS name, username and password of your NextGIS ID and press **Sign in**.

.. figure:: _static/ngm_webgis_login_en.png
   :name: ngm_webgis_login_pic
   :align: center
   :width: 10cm
   
   Adding new Web GIS connection
   
If you don't have a Web GIS, tap **create** on this screen. Your account page will be opened in a browser. From that page you can `create a Web GIS <https://docs.nextgis.com/docs_ngcom/source/create_webgis.html>`_.

**From the Settings**

1. Open Layers tree panel (item 1 in :numref:`ngmobile_main_activity_pic_1`). 
   
2. Select "Settings".

.. figure:: _static/ngm_menu_en.png
   :name: ngmobile_settings2_pic
   :align: center
   :width: 10cm

   Main menu

3. Select "Web GIS".  

.. figure:: _static/ngm_settings_webgis_en.png
   :name: ngmobile_settings_ngw_pic
   :align: center
   :width: 10cm
   
   Settings menu
  
4. In the opened menu press **Add Web GIS**.  
   
.. figure:: _static/ngm_nowebgis_en.png
   :name: ngm_nowebgis_pic
   :align: center
   :width: 10cm

   Web GIS menu

On the next screen enter the Web GIS name, username and password of your NextGIS ID and press **Sign in** (see :numref:`ngm_webgis_login_pic`).



.. _ngm_create_connection_onp:

Add connection to NextGIS Web on-premise
-----------------------------------------------------

.. only:: html
   
   You can learn more about main features of NextGIS Web on-premise 
   in :ref:`ngw_keyfeatures`.

.. only:: latex

   You can learn more about main features of NextGIS Web on-premise 
   in `Key features of NextGIS Web <http://docs.nextgis.com/docs_ngweb/source/general.html#ngweb-keyfeatures>`_.
   
If you keep your data on your own NextGIS Web server, tap "Add Web GIS" using either of the ways to add a new Web GIS connection (see above), then tap the link at the bottom of the screen (see :numref:`ngmobile_new_webgis_nextgis_pic`).

.. figure:: _static/ngm_webgis_switch_op_en.png
   :name: ngmobile_new_webgis_nextgis_pic
   :align: center
   :width: 10cm

   Add Web GIS dialog

In the opened dialog fill in the connection details: Web GIS URL, username and password, then press **Sign in**.

.. figure:: _static/ngm_webgis_login_op_en.png
   :name: ngm_webgis_login_op_pic
   :align: center
   :width: 10cm

   Web GIS connection parameters
      
.. note::
   Many devices automatically add a space at the end of a text field when using  
 auto-complete or pasting from a clipboard.  
 In this case you need to delete the space manually. For NextGIS Web an additional character makes it a different username / password, so you won't be able to log in.

.. _ngmobile_change_account:

Edit Web GIS connection
-------------------------------------

1. Open the menu by tapping the three dots in the top right corner  (item 5 in :numref:`ngmobile_main_activity_pic_1`). 
2. Select "Settings" (:numref:`ngmobile_settings2_pic`).
3. Select "Web GIS" in the opened menu
   (:numref:`ngmobile_settings_ngw_pic`).  
4. Select a Web GIS from the list 
   (see :numref:`ngmobile_settings_ngw_pic`). 
5. On the next screen select "Edit account".

.. figure:: _static/ngm_webgis_edit_acc_en.png
   :name: ngm_webgis_edit_acc_pic
   :align: center
   :width: 10cm
    
   Editing Web GIS connection

6. In the opened window you can modify the following 
fields (see :numref:`ngmobile_edit_account_pic`):

1. Username;
2. Password.

.. figure:: _static/ng_mobile_edit_account_eng.png
   :name: ngmobile_edit_account_pic
   :align: center
   :width: 10cm

   Editing a Web GIS connection

.. _ngmobile_delete_account:

Delete Web GIS connection
-------------------------------

There are two ways to delete a connection to a Web GIS. 

You can delete the connection **in the app settings**.

1. Open the menu by tapping the three dots in the top right corner  (item 5 in :numref:`ngmobile_main_activity_pic_1`). 
2. Select "Settings" (:numref:`ngmobile_settings2_pic`).
3. Select "Web GIS" 
   (:numref:`ngmobile_settings_ngw_pic`).  

4. Select a Web GIS from the list. 
  
   
5. Select "Delete account".

.. figure:: _static/ngm_webgis_remove_acc_en.png
   :name: ngmobile_remove_account1_pic
   :align: center
   :width: 10cm
    
   Delete Web GIS connection
   
6. Confirm deleting the account.

.. figure:: _static/ngm_webgis_remove_confirm_en.png
   :name: ngm_webgis_remove_confirm_pic
   :align: center
   :width: 10cm
    
   Delete Web GIS connection

You can also delete a connection to a Web GIS in your **device settings**.

1. Go to the Settings of your phone or tablet.
2. Go to Accounts section of the settings.

.. figure:: _static/settings_in_os_eng.png
   :name: ngmobile_settings_in_os_pic
   :align: center
   :width: 10cm
   
   Selecting accounts in OS settings
   
3. Select the "NextGIS" account from the list.

.. figure:: _static/accounts_in_os_eng.png
   :name: ngmobile_accounts_in_os_pic
   :align: center
   :width: 10cm
   
   NextGIS account in OS settings

4. Select the Web GIS connection you want to delete.

.. figure:: _static/remove_account_in_os_eng.png
   :name: ngmobile_remove_account_in_os_pic
   :align: center
   :width: 10cm
   
   Selecting Web GIS account in OS settings

Tap **Delete** (it can be on the same page or in a context menu).

.. figure:: _static/remove_account1_in_os_eng.png
   :name: ngmobile_remove_account1_in_os_pic
   :align: center
   :width: 10cm
   
   Deleting Web GIS account through the OS settings
