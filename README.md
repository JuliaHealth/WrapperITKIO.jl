# WrapperITKIO.jl
 provides wrapper functions in Julia from the InsightToolkit Image Registration functions.

Usage::

```
using WrapperITKIO
```

Loading Spatial meta data from an image file path:

```
spatialMeta = WrapperITKIO.loadSpatialMetaData("filepath")

spatialMeta.origin

spatialMeta.spacing

spatialMeta.size

spatialMeta.direction

```

Loading Voxel data from an image file path and spatial meta data

```
voxelData = WrapperITKIO.loadVoxelData("filepath",spatialMeta)
voxelData.dat
```
