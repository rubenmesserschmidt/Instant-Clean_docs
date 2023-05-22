Changelog
#########

|
2.0.0
*****

New Features
^^^^^^^^^^^^

* **Manifold Category**: All new category containing 6 new features to make your mesh manifold, find all details :ref:`here <Manifold>_`.
|

* **Convert to Quads Settings**: Added max face/shape angle threshold settings for better results.
|
* **Remove Double Materials**: Merge material duplicates into a single one (by suffix e.g. material_name.001, material_name.002, ...).
 :Remove Data: Also destructively delete the duplicates from the file to save memory.
|

* **Material Slots Clear Method**: Added two options for the material slot clean.
 :Unused: Remove unused material slots only.
 :All: Remove all material slots, thus removing all materials from the object.
|

* **Merge Panels**: Added the option to merge all panels of my addons into a single panel called *Ruben's Addons*. You'll find the option under the addon preferences (*Edit>Preferences>Add-Ons>Instant Clean*).
|

Bug Fixes
^^^^^^^^^

* **Non-Manifold Faces**: Accelerated the execution speed to the 5X as before.
* **Overall Performance**: Improved the performance of the whole addon by 10-20% depending on the settings you have enabled.

|
1.2.1
*****

* **Bug Fixes**
 :Topology: Fixed an issue where topology to quads was not working when using dissolve at the same time.
 :Repair: Renamed the option 'Interiors' to 'Non-Manifolds'.
|

1.2.0
*****

* **New Features**
 :Clear Custom Split Normals: Clears custom split normals if any available.
 :Clear Sharp Edges: Clears sharp edges i.a. resulting from custom split normals.

* **Bug Fixes**
 :N-Panel: The Instant Clean Panel is now movable by N-Panel manager addons.
|

1.1.0
*****

* **New Features**
 :Weighted Normals: Add *Weighted Normals* modifier to your objects.

* **Bug Fixes**
 :Topology Stats: Increased topology percentage now shows the correct sign.
 :Auto Smooth: Applies *Shade Smooth* now if not already shaded smooth.
 :Normal Stats: Fixed an rare error during the calculation of the results from the *Normal* operations
|
