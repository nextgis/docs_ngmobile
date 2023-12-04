.. _ngmobile_mock_location:

Simulation of location data
=============================================

How to use a third party software as a source of location data for your device.

Install a mock location app. For example, `this one <https://lockito-app.com/>`_.

Turn on Developer mode on your smart phone.
To do so, tap the Build number 7 times (in Software information).

.. figure:: _static/ngm_enter_developer_mode_en.png
   :name: ngm_enter_developer_mode_pic
   :align: center
   :width: 6cm
   
   Enabling developer mode

In the Developer options select mock location app installed on step 1.


.. figure:: _static/ngm_developer_options_en.png
   :name: ngm_developer_options_pic
   :align: center
   :width: 6cm
   
   Opening developer settings

.. figure:: _static/ngm_select_mock_location_app_en.png
   :name: ngm_select_mock_location_app_pic
   :align: center
   :width: 6cm
   
   Selecting mock location app


Open the mock location app.
Create a simulation, name it.

.. figure:: _static/ngm_new_simulation_en.png
   :name: ngm_new_simulation_pic
   :align: center
   :width: 6cm
   
   Creating a simulation



Select a point on the map (or use current location) and tap Play.

.. figure:: _static/ngm_select_point_play_en.png
   :name: ngm_select_point_play_pic
   :align: center
   :width: 6cm
   
   Selecting point on the map

.. figure:: _static/ngm_in_progress_en.png
   :name: ngm_in_progress_pic
   :align: center
   :width: 6cm
   
   Simulation in progress

From that moment on your smart phone will get coordinates of your current location from the app. Open NextGIS Mobile to see that it works.

.. figure:: _static/ngm_simulated_location_en.png
   :name: ngm_simulated_location_pic
   :align: center
   :width: 6cm
   
   Coordinates from an external source in NextGIS Mobile
