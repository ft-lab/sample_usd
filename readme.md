# USD Samples

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

### Up Axis

|File|Material Type|Description|      
|---|---|---|      
|[UpAxis_Y.usda](samples/UpAxis/UpAxis_Y.usda)|OmniPBR|Up axis Y.<br>![UpAxis_Y](samples/UpAxis/images/UpAxis_Y.jpg)|      
|[UpAxis_Z.usda](samples/UpAxis/UpAxis_Z.usda)|OmniPBR|Up axis Z.<br>![UpAxis_Z](samples/UpAxis/images/UpAxis_Z.jpg)|      

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
|[rect_light.usda](samples/light/rect_light.usda)|-|Rect Light.<br>Adjusts the ratio of RectLight area to intensity so that the same amount of light is produced for different sizes.<br>![rect_light](samples/light/images/rect_light.jpg)|      
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
|[payload_use_primPath.usda](samples/reference/payload_use_primPath.usda)|OmniPBR|Specify PrimPath when doing Payload.<br>Refer to<br>[payload_use_primPath.usda](samples/reference/payload_use_primPath.usda) to<br>[refObjects.usda](samples/reference/refObjects.usda)<br>![payload_use_primPath](samples/reference/images/payload_use_primPath.png)|      

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
|[simpleCubeSubdivision.usda](samples/mesh/simpleCubeSubdivision.usda)|-|Mesh Cube with Subdivision.<br>Use faceVarying with normal and UV.<br>![simpleCubeSubdivision.jpg](samples/mesh/images/simpleCubeSubdivision.jpg)|      
|[primvars_normals.usda](samples/mesh/primvars_normals.usda)|OmniPBR|Normals are specified with "primvars:normals".<br>![primvars_normals.jpg](samples/mesh/images/primvars_normals.jpg)|      

### Material

UsdPreviewSurface.    

|File|Material Type|Description|      
|---|---|---|      
|[UsdPreviewSurface.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface.usda)|UsdPreviewSurface|DiffuseColor only.<br>![UsdPreviewSurface.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface.jpg)|      
|[UsdPreviewSurface_texture.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_texture.usda)|UsdPreviewSurface|DiffuseColor Texture.<br>![UsdPreviewSurface_texture.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_texture.jpg)|      
|[UsdPreviewSurface_multiply_texture.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_multiply_texture.usda)|UsdPreviewSurface|DiffuseColor multiply texture.<br>Use inputs:scale.<br>![UsdPreviewSurface_multiply_texture.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_multiply_texture.jpg)|      
|[UsdPreviewSurface_transform.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_transform.usda)|UsdPreviewSurface|DiffuseColor texture with UsdTransform2d.<br>Use inputs:translation, inputs:scale.<br>![UsdPreviewSurface_transform.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_transform.jpg)|      
|[UsdPreviewSurface_transform_rotate.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_transform_rotate.usda)|UsdPreviewSurface|DiffuseColor texture with UsdTransform2d.<br>Use inputs:translation, inputs:scale, inputs:rotation.<br>![UsdPreviewSurface_transform_rotate.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_transform_rotate.jpg)|      
|[UsdPreviewSurface_opacity.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_opacity.usda)|UsdPreviewSurface|Use inputs:opacity.<br>![UsdPreviewSurface_opacity.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_opacity.jpg)<br>Rendered in RTX-Real-Time.<br>Render Settings-Real Time-Ray Tracing-Translucency-Enable Fractional Cutout Opacity : On|      
|[UsdPreviewSurface_opacityThreshold.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_opacityThreshold.usda)|UsdPreviewSurface|Opacity Map, Normal Map.<br>Use inputs:opacityThreshold.<br>![UsdPreviewSurface_opacityThreshold.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_opacityThreshold.jpg)|      
|[UsdPreviewSurface_cyawan.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_cyawan.usda)|UsdPreviewSurface|PBR Material.<br>Use diffuseColor Map, Normal Map, Roughness Map, Occlusion Map.<br>![UsdPreviewSurface_cyawan.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_cyawan.jpg)<br>In NormnalMap, bias=(-1, -1, -1, 0), scale=(2, 2, 2, 1).|      
|[UsdPreviewSurface_vertexColor.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_vertexColor.usda)|UsdPreviewSurface|Vertex Color<br>Supported by USDView, Omniverse RTX (USD Composer 2023.1.1 Beta).<br>![UsdPreviewSurface_vertexColor.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_vertexColor.jpg)|      
|[UsdPreviewSurface_vertexColorFaces.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_vertexColorFaces.usda)|UsdPreviewSurface|Vertex Color<br>Supported by USDView, Omniverse RTX (USD Composer 2023.1.1 Beta).<br>![UsdPreviewSurface_vertexColorFaces.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_vertexColorFaces.jpg)|      
|[UsdPreviewSurface_emissive_texture.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_emissive_texture.usda)|UsdPreviewSurface|Use emissiveColor Texture.<br>![UsdPreviewSurface_emissive_texture.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_emissive_texture.jpg)|      
|[UsdPreviewSurface_clearcoat.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_clearcoat.usda)|UsdPreviewSurface|Use clearcoat, clearcoatRoughness.<br>![UsdPreviewSurface_clearcoat.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_clearcoat.jpg)|      
|[UsdPreviewSurface_clearcoat_with_texture.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_clearcoat_with_texture.usda)|UsdPreviewSurface|Use clearcoat(with texture), clearcoatRoughness.<br>![UsdPreviewSurface_clearcoat_with_texture.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_clearcoat_with_texture.jpg)|      
|[UsdPreviewSurface_clearcoat_with_texture2.usda](samples/Material/UsdPreviewSurface/UsdPreviewSurface_clearcoat_with_texture2.usda)|UsdPreviewSurface|Use clearcoat(with texture), clearcoatRoughness(with texture).<br>![UsdPreviewSurface_clearcoat_with_texture2.jpg](samples/Material/UsdPreviewSurface/images/UsdPreviewSurface_clearcoat_with_texture2.jpg)|      


OmniPBR.    

|File|Material Type|Description|      
|---|---|---|      
|[UsdPreviewSurfaceAndOmniPBR.usda](samples/Material/OmniPBR/UsdPreviewSurfaceAndOmniPBR.usda)|OmniPBR|DiffuseColor only.<br>Comparison of UsdPreviewSurace and OmniPBR, where DIffuseColor is stored as "Linear".![UsdPreviewSurfaceAndOmniPBR.jpg](samples/Material/OmniPBR/images/UsdPreviewSurfaceAndOmniPBR.jpg)|      
|[OmniPBR_cyawan.usda](samples/Material/OmniPBR/OmniPBR_cyawan.usda)|OmniPBR|AlbedoMap, RoughnessMap, NormalMap, and OcclusionMap in OmniPBR.<br>![OmniPBR_cyawan.jpg](samples/Material/OmniPBR/images/OmniPBR_cyawan.jpg)|      
|[OmniPBR_opacity.usda](samples/Material/OmniPBR/OmniPBR_opacity.usda)|OmniPBR|Use Opacity.<br>![OmniPBR_opacity.jpg](samples/Material/OmniPBR/images/OmniPBR_opacity.jpg)<br>Rendered in RTX-Real-Time.<br>Render Settings-Real Time-Ray Tracing-Translucency-Enable Fractional Cutout Opacity : On|      
|[OmniPBR_opacityThreshold.usda](samples/Material/OmniPBR/OmniPBR_opacityThreshold.usda)|OmniPBR|Use OpacityMap.<br>Specify "mono_alpha" in Opacity Mono Source.<br>![OmniPBR_opacityThreshold.jpg](samples/Material/OmniPBR/images/OmniPBR_opacityThreshold.jpg)|      
|[OmniPBR_multiply_texture.usda](samples/Material/OmniPBR/OmniPBR_multiply_texture.usda)|OmniPBR|DiffuseColor multiply texture.<br>![OmniPBR_multiply_texture.jpg](samples/Material/OmniPBR/images/OmniPBR_multiply_texture.jpg)|      
|[OmniPBR_emissive_intensity.usda](samples/Material/OmniPBR/OmniPBR_emissive_intensity.usda)|OmniPBR|Use Emissive. Comparison of emissive_intensity.<br>![OmniPBR_emissive_intensity.jpg](samples/Material/OmniPBR/images/OmniPBR_emissive_intensity.jpg)|      
|[OmniPBR_emissive_texture.usda](samples/Material/OmniPBR/OmniPBR_emissive_texture.usda)|OmniPBR|Use emissiveColor Texture.<br>![OmniPBR_emissive_texture.jpg](samples/Material/OmniPBR/images/OmniPBR_emissive_texture.jpg)|      

### DisplayColor      
|File|Material Type|Description|      
|---|---|---|      
|[displayColor.usda](samples/DisplayColor/displayColor.usda)|---|Set DisplayColor of single color.<br>![displayColor.jpg](samples/DisplayColor/images/displayColor.jpg)|      
|[displayColor_VertexColor.usda](samples/DisplayColor/displayColor_VertexColor.usda)|---|Set the vertex color with DisplayColor.<br>![displayColor_VertexColor.jpg](samples/DisplayColor/images/displayColor_vertexColor.jpg)<br>Works with Omniverse RTX, USDView.|      
|[displayColor_VertexColorFaces.usda](samples/DisplayColor/displayColor_VertexColorFaces.usda)|---|Set the vertex color with DisplayColor. For each face.<br>![displayColor_VertexColorFaces.jpg](samples/DisplayColor/images/displayColor_VertexColorFaces.jpg)<br>Works with Omniverse RTX, USDView.|      

### Points (Point Clouds)

|File|Material Type|Description|      
|---|---|---|      
|[PointClouds.usda](samples/PointClouds/PointClouds.usda)|---|Point Clouds.<br>![PointClouds.jpg](samples/PointClouds/images/PointClouds.jpg)<br>Supported by USDView.<br>Omniverse RTX does not reflect DisplayColor to the point.|      

### Display Name

The specified DisplayName is used as the Prim name in the UI display.     
DisplayName is not bound by any single-byte alphanumeric character or name prefix constraints.     

|File|Material Type|Description|      
|---|---|---|      
|[DisplayName.usda](samples/DisplayName/DisplayName.usda)|---|When UTF-8 Japanese is specified as DisplayName.<br>![DisplayName.png](samples/DisplayName/images/DisplayName.png)<br>Supported by USDView.<br>DisplayName in Japanese (UTF-8) in Omniverse can be optionally displayed, but the font must be specified.<br>This will be kept private.|      
|[DisplayName_english.usda](samples/DisplayName/DisplayName_english.usda)|---|When English is specified as DisplayName.<br>![DisplayName_english.png](samples/DisplayName/images/DisplayName_english.png)<br>In the Stage window, select "Show Display Names" from the Options menu and set it to On.|      

### Layer

|File|Material Type|Description|      
|---|---|---|      
|[layer1.usda](samples/Layer/layer1.usda)|UsdPreviewSurface|sublayer_sphere.usda of the sublayer from layer1.usda.<br>![layer1.jpg](samples/Layer/images/layer1.jpg)|      
|[layer1_override.usda](samples/Layer/layer1_override.usda)|UsdPreviewSurface|sublayer_sphere.usda of the sublayer from layer1_override.usda.<br>Also, an override was performed in layer1_override.usda.<br>![layer1_override.jpg](samples/Layer/images/layer1_override.jpg)|      

### Kind

|File|Material Type|Description|      
|---|---|---|      
|[kind.usda](samples/kind/kind.usda)|---|Use kind.<br>![kind.jpg](samples/kind/images/kind.jpg)|      

## Knowledges

* [Color space : Interconversion between sRGB and Linear(raw)](./knowledges/ColorSpaceConversion.md)
* [Lights](./knowledges/Lights.md)
* [Lighting Calculation](./knowledges/LightingCalculation.md)
* Camera

----

