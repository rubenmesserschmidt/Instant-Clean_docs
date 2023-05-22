Operation Categories
##########

| Every operation category can be enabled/disabled by checking/unchecking it's header.
| It's also possible to execute them seperated from each other by pressing the *Play* button right next to the header.
|

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

Manifold
********

* **Remove Non-Manifold Faces**: Dissolve faces which have edges connected to more than two faces such as interior faces.
* **Remove Non-Manifold Verts**: Split vertices which are connecting parts of the mesh in a zero volume point.
* **Wire Geometry**: Dissolve edges which are not connected to any faces.
* **Fill Holes**: Fill up holes in the mesh.
 :Max Sides: Only holes with a lower amount of sides will be filled.
* **Flatten Faces**: Flatten faces which vertices are not in the same plane by moving them to match an average plane.
 :Factor: Determines how strong vertices will be moved to make all faces as flat as possible (higher is stronger).
 :Iterations: Repeat the flatten process this number of times (more often makes the faces flatter).
* **Undistort Faces**: Triangulate non-planar faces to create as many planar faces as possible.
 :Max Angle: Triangulate only faces whose normal and any loops normal of the face having a higher angle than this between them (higher values triangulating fewer faces).
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
* **Weighted Normals**: Add *Weighted Normals* modifier to your objects.
|

Objectdata
**********

* **Remove Double Materials**: Merge material duplicates into a single one (by suffix e.g. material_name.001, material_name.002, ...).
 :Remove Data: Also destructively delete the duplicates from the file to save memory.
* **Material Slots**: Removes material slots based on a clear method.
 :Unused: Remove unused material slots only.
 :All: Remove all material slots, thus removing all materials from the object.
* **Vertex Groups**: Removes all vertex groups which have no vertices assigned to it.
|


