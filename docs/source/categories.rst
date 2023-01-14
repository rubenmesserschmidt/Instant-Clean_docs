Categories
##########

Repair
******

* **Loose**: Dissolves Unconnected Geometry.
 :Vertices: Vertices which are not part of an edge.
 :Edges: Edges which are not part of an face.
 :Faces: Faces which are not connected to other faces.
* **Doubles**: Vertices with the same position.
 :Max Distance: Maximum Distance between positions to be considered as same.
* **Zero Faces**: Faces with an area of zero.
 :Max Area: Maximal area of an face to be considered as zero.
* **Dispensables**: Vertices which are connecting two edges by an angle of zero.
 :Max Distance: Maximum angle between two edges to be considered as zero.
* **Interiors**: Faces which are inside the mesh.
|

Dissolve
********

* **Max Angle**: Maximal angle at which geometry will be dissolved.
* **Boundaries**: Dissolve edges which are part of one face only.
* **Protect**: Keep edges with certain dependencies or attributes.
 :Sharp: Keep edges marked as sharp.
 :Seam: Protects edges marked as seam.
 :UV: Keep edges which are boundary of UV islands.
 :Materials: Keep edges which delimit two different assigned materials.
|

Topology
********

* **Type**: Type of topology which the mesh will be converted to.
 :Tris: Triangulates all faces.
 * **Methods**: Which algorithm to choose for triangulation.
  :Quad Method: Method which will be used for the quad to triangle computation.
  :NGon Method: Method which will be used for the ngon to triangle computation.
 :Quads: Converts faces to quads if possible.
 * **Compare**: Keep edges with certain dependencies or attributes
  :Sharp: Keep edges marked as sharp.
  :Seam: Keep edges marked as seam.
  :VCol: Keep vertex colors.
  :UV: Keep edges which are boundary of UV islands.
  :Material: Keep edges which delimit two different assigned materials.
|

Normals
*******

* **Recalculate**: Recalculate the normal of each face.
 :Outside: Outside of each face is outside of the mesh.
 :Inside: Outside of each face is inside of the mesh.
* **Auto Smooth**: Apply an angle restricted smooth shading.
 :Max Angle: Maximum angle for smooth shading.
|

Objectdata
**********

* **Material Slots**: Removes all material slots whose materials are not assigned to any part of the mesh.
* **Vertex Groups**: Removes all vertex groups which have no vertices assigned to it.
|


