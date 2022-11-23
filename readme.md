USD samples.     
This includes materials using MDLs that are compatible with NVIDIA Omniverse.      

## What USD ?

Pixar has defined a file format called "Universal Scene Description (USD)".     
https://graphics.pixar.com/usd/release/index.html

USD is more than a file format; it also acts as a framework for defining 3D scenes.     

## USD samples

I have decided to create a sample of USD files by function.     

### defaultPrim

|File|Material Type|Description|      
|---|---|---|      
|[not_used_defaultPrim.usda](samples/defaultPrim/not_used_defaultPrim.usda)|OmniPBR|Do not use defaultPrim<br>![use_defaultPrim](samples/defaultPrim/images/use_defaultPrim.jpg)|      
|[use_defaultPrim.usda](samples/defaultPrim/use_defaultPrim.usda)|OmniPBR|Use of defaultPrim<br>![use_defaultPrim](samples/defaultPrim/images/use_defaultPrim.jpg)|      

### Hierarchy

|File|Material Type|Description|      
|---|---|---|      
|[MultipleRoots.usda](samples/hierarchy/MultipleRoots.usda)|OmniPBR|Scene with more than one root.<br>Also, defaultPrim is not specified.<br>![MultipleRoots](samples/hierarchy/images/MultipleRoots.png)|      

### metersPerUnit

|File|Material Type|Description|      
|---|---|---|      
|[unit_test_cm.usda](samples/metersPerUnit/unit_test_cm.usda)|OmniPBR|Placement of 1 meter plane.<br>Stage unit is cm (default.metersPerUnit=0.01).<br>![unit_test_cm](samples/metersPerUnit/images/unit_test_cm.jpg)|      
|[unit_test_m.usda](samples/metersPerUnit/unit_test_m.usda)|OmniPBR|Placement of 1 meter plane.<br>Stage unit is m (metersPerUnit=1.0).<br>![unit_test_m](samples/metersPerUnit/images/unit_test_m.jpg)|      
|[unit_test_mm.usda](samples/metersPerUnit/unit_test_mm.usda)|OmniPBR|Placement of 1 meter plane.<br>Stage unit is mm (metersPerUnit=0.001).<br>![unit_test_mm](samples/metersPerUnit/images/unit_test_mm.jpg)|      


### Primitive

|File|Material Type|Description|      
|---|---|---|      
|[simple_primitives.usda](samples/primitive/simple_primitives.usda)|-|Placement of Cube,Sphere,Cylinder,Capsule,Cone<br>![simple_primitives](samples/primitive/images/simple_primitives.jpg)|      

### Curves

|File|Material Type|Description|      
|---|---|---|      
|[basisCurves.usda](samples/curves/basisCurves.usda)|-|BasisCurves<br>![basisCurves](samples/curves/images/basisCurves.jpg)|      

### Light

|File|Material Type|Description|      
|---|---|---|      
|[point_light.usda](samples/light/point_light.usda)|-|Point Light with Sphere Light.<br>Use the ratio of radius to surface area to achieve the same light intensity<br>![point_light](samples/light/images/point_light.jpg)|      
|[spot_light.usda](samples/light/spot_light.usda)|-|Spot Light with Sphere Light.<br>Change in Cone Angle and Cone Softness.<br>![spot_light](samples/light/images/spot_light.jpg)|      
|[dome_light.usda](samples/light/dome_light.usda)|OmniPBR|DomeLight.<br>![dome_light](samples/light/images/dome_light.jpg)|      

### doubleSided

|File|Material Type|Description|      
|---|---|---|      
|[doubleSided.usda](samples/doubleSided/doubleSided.usda)|UsdPreviewSurface|DoubleSided.<br>![doubleSided](samples/doubleSided/images/doubleSided.jpg)|      

### Variant

|File|Material Type|Description|      
|---|---|---|      
|[VariantTest.usda](samples/variant/VariantTest.usda)|OmniPBR|Use Variant.<br>Switch chairs.<br>![VariantTest](samples/variant/images/VariantTest.jpg)<br>Shapes and textures are called from external sources.|      


### PointInstancer

|File|Material Type|Description|      
|---|---|---|      
|[point_instancer_01.usda](samples/PointInstancer/point_instancer_01.usda)|UsdPreviewSurface|PointInstancer.<br>![point_instancer_01](samples/PointInstancer/images/point_instancer_01.jpg)|      

### Skeleton

|File|Material Type|Description|      
|---|---|---|      
|[jointTest.usda](samples/Skeleton/jointTest.usda)|OmniPBR|Skin + Joint.<br>![jointTest](samples/Skeleton/images/jointTest.jpg)|      

### Reference, Payload

|File|Material Type|Description|      
|---|---|---|      
|[simple_mesh_sphere_reference.usda](samples/reference/simple_mesh_sphere_reference.usda)|OmniPBR|Refer to [simple_mesh_sphere_reference.usda](samples/reference/simple_mesh_sphere_reference.usda) to [simple_mesh_sphere.usda](samples/reference/simple_mesh_sphere.usda)<br>![simple_mesh_sphere_reference](samples/reference/images/simple_mesh_sphere_reference.jpg)|      
|[simple_mesh_sphere_payload_nest.usda](samples/reference/simple_mesh_sphere_payload_nest.usda)|OmniPBR|Refer with Payload to two levels.<br>[simple_mesh_sphere_payload_nest.usda](samples/reference/simple_mesh_sphere_payload_nest.usda)<br>[simple_mesh_sphere_payload.usda](samples/reference/simple_mesh_sphere_payload.usda)<br>[simple_mesh_sphere.usda](samples/reference/simple_mesh_sphere.usda)<br>![simple_mesh_sphere_payload_nest](samples/reference/images/simple_mesh_sphere_payload.jpg)|      

### Instance

|File|Material Type|Description|      
|---|---|---|      
|[instance_test.usda](samples/instance/instance_test.usda)|-|Use Instance.<br>![instance_test](samples/instance/images/instance_test.jpg)|      

### Mesh

|File|Material Type|Description|      
|---|---|---|      
|[simpleCube.usda](samples/mesh/simpleCube.usda)|-|Mesh Cube.<br>normal and UV with interpolation=faceVarying.<br>![simpleCube.usda](samples/mesh/images/simpleCube.jpg)|      
|[simpleCubeVertex.usda](samples/mesh/simpleCubeVertex.usda)|-|Mesh Cube.<br>normal and UV with interpolation=vertex.<br>![simpleCubeVertex.usda](samples/mesh/images/simpleCubeVertex.jpg)|      
|[concave_polygons.usda](samples/TriangulationOfPolygon/concave_polygons.usda)|UsdPreviewSurface|Triangulation of polygons.<br>Below is the display in Unity.<br>![concave_polygons](samples/TriangulationOfPolygon/images/concave_polygons.jpg)<br>This sample is not correctly triangulated even with Omniverse Create 2022.3.|      
|[easyChair_01.usdc](samples/TriangulationOfPolygon/easyChair_01.usdc)|UsdPreviewSurface|Triangulation of polygons.<br>Below is the display in Unity.<br>![easyChair_01.usdc](samples/TriangulationOfPolygon/images/easyChair_01.jpg)<br>This sample is not correctly triangulated even with Omniverse Create 2022.3.|      
|[simpleCubeSubdivision.usda](samples/mesh/simpleCubeSubdivision.usda)|-|Mesh Cube with Subdivision.<br>Use faceVarying with normal and UV.<br>![simpleCubeSubdivision.usda](samples/mesh/images/simpleCubeSubdivision.jpg)|      

----
