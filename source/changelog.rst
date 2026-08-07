.. _sysadmin_updates:

Changelog
=========

**3.2.1 released on 05 Aug 2026**

* Require confirmation before deleting a newly created or modified object
* Fixed an unnecessary dialog when opening NGRC
* Fixed an unnecessary prompt to save changes when there are no changes


**3.2.0 released on 30 Jul 2026**

* Support for the MBTiles format for local raster layers
* Customizable label colors for polygons and lines
* Go to coordinates tool
* Replace the object deletion popup with a confirmation dialog
* Link to the Web GIS administrator contact form when the user has insufficient permissions
* Use the NGRC file name as the layer name
* Fixed a synchronization error when submitting data with an empty date
* Fixed an issue where the date could not be entered through the form
* Fixed the track visibility toggle state not being displayed correctly
* Fixed an error when attempting to download a non-image attachment from NGW
* Fixed unnecessary text centering in the feature table
* Fixed track visibility toggle not working
* Fixed track display color changes not being applied
* Fixed NGW layer properties enabling auto-sync unexpectedly
* Renamed "Your UID" to "Device ID" to match the Web GIS
* Fixed incorrect rendering of the ruler enable checkbox

**3.1.2 released on 14 Jul 2026**

* Removed all extent requests while adding a raster layer
* Fixed incorrect indication of synchronization flag under Web GIS settings

**3.1.1 released on 08 Jul 2026**

* Added a clear error message instead of “Account is null” when attempting to add a layer
* Added a notification when a form field cannot be used for input
* Added support for selecting a label attribute for feature identification
* The ruler tool is now enabled by default
* Fixed unintended geometry changes when the user did not edit the geometry
* Fixed point features being moved to the current location during creation
* Fixed multiple requests being sent for the same layer
* Fixed the incorrect “Contains ads” label in Google Play
* Added Sentry profiling configuration
