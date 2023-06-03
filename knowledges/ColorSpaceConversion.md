# Color Space Conversion

Colors in USD are unified in the Linear (raw) color space.     
Since the colors you see on a display are sRGB, in most cases you will need to convert from sRGB to Linear.      

Here is the code to convert between sRGB and Linear in Python.      

## References

* https://en.wikipedia.org/wiki/SRGB

## Linear to sRGB

```python
from pxr import Usd, UsdGeom, UsdPhysics, UsdShade, Sdf, Gf, Tf
import math

def _LinearToSRGB(value : float):
    if value <= 0.0031308:
        return value * 12.92
    value = math.pow(value, 1.0 / 2.4) * 1.055 - 0.055
    return value

def LinearToSRGB(colorV : Gf.Vec3f):
    rV = _LinearToSRGB(colorV[0])
    gV = _LinearToSRGB(colorV[1])
    bV = _LinearToSRGB(colorV[2])
    return Gf.Vec3f(rV, gV, bV)
```

## sRGB to Linear

```python
from pxr import Usd, UsdGeom, UsdPhysics, UsdShade, Sdf, Gf, Tf
import math

def _SRGBToLinear(value : float):
    if value <= 0.04045:
        return value / 12.92
    value = math.pow((value + 0.055) / 1.055, 2.4)
    return value

def SRGBToLinear(colorV : Gf.Vec3f):
    rV = _SRGBToLinear(colorV[0])
    gV = _SRGBToLinear(colorV[1])
    bV = _SRGBToLinear(colorV[2])
    return Gf.Vec3f(rV, gV, bV)
```

## Test code

After stating the above, please do the following.    

```python
v1 = Gf.Vec3f(0.75, 0.9, 1.0)
v2 = SRGBToLinear(v1)
v3 = LinearToSRGB(v2)

print(f"v1 = {v1}")
print(f"v2 = {v2}")
print(f"v3 = {v3}")
```

The output is as follows: v1=v3.     
```
v1 = (0.75, 0.9, 1)
v2 = (0.52252156, 0.7874122, 1)
v3 = (0.75, 0.9, 1)
```
