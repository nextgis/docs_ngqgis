DumpLoadField
=============

Fill in string fields of a vector layer from a text file. This plugin is helpful when you need to fill in an empty field or replace values of a field.

Also DumpLoadField can save the contents of a field from an attribute table as TXT file.

After installation you can find the plugin in the Vector menu.

.. _ngq_dumploadfield_add:

Add text field to vector layer attributes
----------------------------------------------------------------

1. Create a new string field in the vector layer attribute table. Save the changes.

2. Open the plugin from :menuselection:`Vector ‣ DumpLoadField ‣ Load to a field`.

3. Select the field you want to fill in.

4. Select a TXT file. In the file the text rows must be in the same order as the layer features.

.. _ngq_dumploadfield_save:

Download text values of an attribute
--------------------------------------------

1. Open the layer in QGIS.

2. In the Menu bar select :menuselection:`Vector ‣ DumpLoadField ‣ Dump a field`.

3. Select the field the contents of which you want to save.

4. Enter a name for the output file.

The values of the string field will be saved to a TXT file.

Check out how the plugin works in our video:

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/gjQCkNLbxUg?si=GKCPqwujg9kMATVE" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch on `youtube <https://youtu.be/gjQCkNLbxUg?si=L7bfWabH0QHMMsVh>`_.
