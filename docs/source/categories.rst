Categories
##########

Repair
******

* **Loose**: Dissolves Unconnected Geometry.
 :Vertices: Vertices which are not part of an edge
 :Edges: Edges which are not part of an face
 :Faces: Faces which are not connected to other faces
* **Doubles**: Vertices with the same position
 :Max Distance: Maximal Distance between positions to be considered as same
* **Zero Faces**: Faces with an area of zero
 :Max Area: Maximal area of an face to be considered as zero
* **Dispensables**: Vertices which are connecting two edges by an angle of zero
 :Max Distance: Maximal angle between two edges to be considered as zero
* **Interiors**: Faces which are inside the mesh
|

Dissolve
********

* **Max Angle**: Maximal angle at which geometry will be dissolved.
* **Boundaries**: Dissolve edges which are part of one face only.
* **Protect**: Ignore edges with certain dependencies or attributes.
 :Sharp: Protects edges marked as sharp.
 :Seam: Protects edges marked as seam.
 :UV: Protects edges which are boundary of UV islands.
 :Materials: Protects edges which delimit two different assigned materials.
|

Topology
********

* **Type**: Type of topology which the mesh will be converted to.
 :Tris: Triangulates all faces.
 * **Methods**: Which algorithm to choose for triangulation.
  :Quad Method: Method which will be used for the quad to triangle computation.
 :Quads: Converts faces to quads if possible.
Normals
*******

Objectdata
**********


