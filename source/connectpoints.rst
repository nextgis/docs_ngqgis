Connect Points
==============

Create lines connecting two point layers using matching attribute values.

Points in one layer are matched to points in another layer with the same value of the specified numeric attribute (e.g. id).

After installation you'll find the plugin in the Plugins toolbar: |button_connectpoints|.

.. |button_connectpoints| image:: _static/button_connectpoints.png
   :width: 8mm

First open the plugin Settings dialog from its dropdown menu:

* Select layer FROM;
* Select layer TO;
* Select ID field in the FROM layer;
* Link field - select the field in the FROM that contains the value to be matched with the attribute in the TO layer;
* Select ID field in the TO layer;
* Choose the way to save the result: select an existing line layer of the project or enter a name to create a new layer.

Press **Ok** to save the settings.

In the plugin dropdown menu select **Connect points**. Plugin will generate lines that link the points of the FROM layer to points of the TO layer, with indicated direction.

See how the plugin works in our video:

.. raw:: html

   <iframe width="560" height="315" src="https://www.youtube.com/embed/enD5z4mwsfg?si=ZcRWczPGinhhuKDa" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

Watch on `youtube <https://youtu.be/enD5z4mwsfg?si=CRV60Tm7xaNLVPyY>`_.
