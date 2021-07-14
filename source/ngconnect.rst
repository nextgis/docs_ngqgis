.. sectionauthor:: Екатерина Петруненко <ekaterina.petrunenko@nextgis.com>

.. _ng_connect:
    
NextGIS Connect
===============

This plugin allows QGIS user to upload and download resources to and from Web GIS or NextGIS Web (further both refer as “Web GIS”) directly from QGIS interface.

With NextGIS Connect you can:

1.	Download geodata from Web GIS to desktop GIS. 
2.	Upload vector and raster layers from desktop GIS to Web GIS.
3.	Upload whole QGIS projects to Web GIS , including styles, layer hierarchy, etc.
4.	Create WFS service in one click and edit data directly in Web GIS.


.. important::

If you plan to share large data through NextGIS Connect, you might need to configure QGIS timeouts for network requests. This setting is in the menu section **Settings** -> **Options** -> **Network** -> Timeout for network requests (ms). The recommended value is **300,000**, it can be increased if necessary.


.. warning::

   **Photos** made via NextGIS Collector/Mobile apps and uploaded to Web GIS as attachments to layers **wouldn’t be available** in desktop NextGIS QGIS after downloading these layers through NextGIS Connect plugin.
   Here is a guide how to change layer’s style and not to lose attached photos:
   
1.	Download target layer into NextGIS QGIS via Connect.
2.	Change style of the layer (colour, line width, etc.)
3.	Click on **Update style** through selecting **Style** of the target resource in right panel.

After these steps old style of the target layer will be deleted from Web GIS and the new style will be uploaded; all attachments remain untouched. 

Connect plugin is a part of NextGIS QGIS distributive and ready to go right after installation of desktop app. Plugin is also available through official QGIS repository, so it can be launched in other QGIS compilations.   

When plugin is installed its icon appears in a toolbar:

.. figure:: _static/nextgis_connect/logo.png
   :align: center

Clicking on the icon calls NextGIS Connect panel.

.. figure:: _static/nextgis_connect/panel.png
   :align: center

If no connection is set at the moment, corresponding message will be shown.

.. figure:: _static/nextgis_connect/panel_no_connections.png
   :align: center

Create a Connection
-------------------------

To create a connection you need to know an address of a target Web GIS. For instance, if you’ve created your own Web GIS, its address can be found on https://my.nextgis.com/webgis page. 

.. figure:: _static/nextgis_connect/my_nextgis.png
   :align: center

Click on “Settings” button in NextGIS Connect panel.

.. figure:: _static/nextgis_connect/call_settings.png
   :align: center

In pop-up window press on “New” and fill in the fields:

1.	URL – address of a target Web GIS.
2.	Name – connection id, how it will be shown in the list of connections.

If you want to perform actions that need special permission, uncheck box next to “As guest” and fill in “Login” and “Password” fields. For example, unauthorized users usually can’t create or delete resources.

.. figure:: _static/nextgis_connect/connection_settings.png
   :align: center

Press “OK”. In “Settings” window from the drop-down list select a connection you want to activate.

Main Settings
-------------------------

.. figure:: _static/nextgis_connect/settings.png
   :align: center

1. Rename forbidden fields – while uploading layer itself or as a part of a project, plugin renames fields forbidden for Web GIS.

2. Fix incorrect geometries – while uploading layer itself or as a part of a project, plugin transforms geometries into same type.

3. Abort project import after first layer import failure – plugin wouldn’t keep on uploading project if any layer is failed to be imported into Web GIS.

4. Open web map automatically on creation – after successful import of a project into Web GIS, web map will be created and automatically opened in browser. 

5. Add WFS layer to QGIS on WFS service creation – after creation of WFS service in Web GIS it will be automatically added to QGIS as a layer.

Resource Types
-------------------------
.. |resource_vector_point| image:: _static/nextgis_connect/vector_layer_point.png
.. |resource_vector_mpoint| image:: _static/nextgis_connect/vector_layer_mpoint.png
.. |resource_vector_line| image:: _static/nextgis_connect/vector_layer_line.png
.. |resource_vector_mline| image:: _static/nextgis_connect/vector_layer_mline.png
.. |resource_vector_polygon| image:: _static/nextgis_connect/vector_layer_polygon.png
.. |resource_vector_mpolygon| image:: _static/nextgis_connect/vector_layer_mpolygon.png
.. |resource_wfs| image:: _static/nextgis_connect/resource_wfs.png
.. |resource_wms| image:: _static/nextgis_connect/resource_wms.png
.. |resource_style| image:: _static/nextgis_connect/resource_style.png
.. |resource_webmap| image:: _static/nextgis_connect/resource_webmap.png
.. |resource_group| image:: _static/nextgis_connect/resource_group.png
- |resource_vector_point| - Point vector layer (NGW Vector Layer)
- |resource_vector_mpoint| - Multipoint vector layer (NGW Vector Layer)
- |resource_vector_line| - Line vector layer (NGW Vector Layer)
- |resource_vector_line| - Multiline vector layer (NGW Vector Layer)
- |resource_vector_polygon| - Polygon vector layer (NGW Vector Layer)
- |resource_vector_mpolygon| - Multipolygon vector layer (NGW Vector Layer)
- |resource_style| - Vector layer style. QGIS style gets "(qgis)" prefix, MapServer style - "(ms)"
- |resource_wfs| - WFS Service (NGW WFS Service)
- |resource_wms| - WMS Service (NGW WMS Service)
- |resource_webmap| - Web map (NGW Web Map)
- |resource_group| - Resource group (NGW Web Map)

Available Operations
-----------------------

*Add to QGIS*

.. figure:: _static/nextgis_connect/add_to_qgis.png
   :align: center

Option is available if one of the following resources is selected in NextGIS Web resource tree:

- Vector layer (NGW Vector Layer) |resource_vector| - GeoJSON vector layer will be created in QGIS.
- WFS service (NGW WFS Service) |resource_wfs| - WFS layer will be created in QGIS.
- QGIS style of a vector layer |resource_style| - GeoJSON vector layer with the style identical to selected one will be created in QGIS.

.. |resource_vector| image:: _static/nextgis_connect/resource_vector.png

.. |resource_wfs| image:: _static/nextgis_connect/resource_wfs.png

*Add to Web GIS*

.. figure:: _static/nextgis_connect/add_to_ngw.png
   :align: center

Option “Import selected layer(s)” is available if one of the following resources is selected in QGIS Layers Panel:

- Vector layer – vector layer with its style will be imported into Web GIS. Style can be added directly on web map.
- Raster layer – raster layer with a default style will be created in Web GIS. Style can be added directly on web map.

Option “Import/Update style” is available when vector layer is selected in QGIS Layers Panel. Select two vector layers: in resource tree and in QGIS Layer Panel.  This operation copies style from the layer in QGIS and assigns it to the selected layer in Web GIS resource tree.


Option “Import current project” is always available. All layers for which option “Import selected layer(s)” is available will be added to Web GIS, as well as all groups with retained hierarchy from QGIS Layers Panel. Also web map will be created and all imported layers will be added to it retaining hierarchy and visibility of QGIS Layers Panel. While importing a project you need to specify the name of the new resource group which will be created in Web GIS. This group will hold all resources imported along with a project. Upon project import created web map will be opened automatically if corresponding option is selected in plugin settings.

Imported resources will be added to a group selected in NextGIS Connect panel. If other type of resources but a group is selected, import will be performed to a closest parent group to selected resource. If no resource is selected, import will be performed to the root directory.

*Create new resource group*

.. figure:: _static/nextgis_connect/create_group.png
   :align: center

Option is available to everyone.
New group will be created in resource group selected via NextGIS Connect panel. If other type of resources but a group is selected, group will be created in a closest parent group to selected resource. If no resource is selected, group will be created in the root directory.

*Refresh resource tree*

.. figure:: _static/nextgis_connect/reload.png
   :align: center

Option updates all resource tree.

*Open map in browser*

.. figure:: _static/nextgis_connect/open_webmap.png
   :align: center

Option is available if web map (NGW Web Map) |resource_webmap|  is selected in NextGIS Connect resource tree. Map will be opened in a new tab of default browser.

.. |resource_webmap| image:: _static/nextgis_connect/resource_webmap.png

*Overwrite selected layer*

Option is available for vector layer in NextGIS Connect resource tree.
Select two vector layers: in resource tree and in QGIS Layer Panel.  This operation deletes all objects from resource tree layer and uploads to it objects from local QGIS layer.

Context Menu
-----------------------
Context menu may differ depending on resource type.

.. figure:: _static/nextgis_connect/context_menu.png
   :align: center

Common options:

-	Open in WebGIS – open page with selected resource in Web GIS;

-	Rename – rename resource;

-	Delete – delete resource.


Variable options – depend on resource type:

-	Add to QGIS – option is described above;

-	Create Web Map – available for resources: Vector layer, Vector layer style, Raster layer;

-	Download as QML – available only for QGIS vector layer style.

