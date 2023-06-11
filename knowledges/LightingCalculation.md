# Lighting Calculation

This section provides the information necessary for lighting calculations.     

## Lighting Unit

|Name|Unit|Description|     
|---|---|---|     
|Illuminace|Lux, lm/m^2|Incident brightness per unit area receiving light|     
|Luminous intensity|cd, lm/sr (sr=Steradian)|Amount of light emitted within a unit solid angle|     
|Luminous flux|lm|Amount of light per unit time; 4Pi*cd for omni-directional as in PointLight|     
|Luminance|cd/m^2, nit|Brightness per unit area viewed from a certain direction|     

### Illuminace

Illuminance is the brightness incident per unit area receiving light.      
The unit is "lux".     
![light_Illuminace.jpg](./images/Lights/light_Illuminace.jpg)     
When luminous flux is *phi* and area is *S* (unit is m^2), illuminance *E* can be calculated by the following equation.

> *E* = *phi* / *S*

### Luminous intensity

It refers to the amount of light emitted within a unit solid angle.    
The unit is "cd (candela)".    
![light_LuminousIntensity.jpg](./images/Lights/light_LuminousIntensity.jpg)     
When the luminous flux is *phi* and the solid angle is *omega* (unit is sr), the luminous intensity *I* can be calculated by the following equation.     

> *I* = *phi* / *omega*

The "solid angle" is not a two-dimensional angle, but a three-dimensional element.     
The area cut off from the conical surface of a sphere of radius 1.0 is called the solid angle.     
![light_SolidAngle.jpg](./images/Lights/light_SolidAngle.jpg)     
If all spheres of radius 1.0 are covered, the surface area of the sphere, "4 * Pi * R^2 = 4Pi", is the solid angle.     

When light is emitted, it is not a uniform luminous flux value in all directions; the intensity of the light may vary depending on the direction.     
Luminous intensity is used to describe this.
The term "light distribution" describes the distribution of luminous intensity.     

### Luminous flux

Luminous flux represents the amount of light per unit time.     
Since light has a direction, a light source such as a light bulb emits light radially.     
The unit is "lm (lumen)".    
![light_LuminousFlux.jpg](./images/Lights/light_LuminousFlux.jpg)     

### Luminance

Luminance represents the (apparent) brightness per unit area as seen from a certain direction.     
The unit is "cd/m^2".     
When the luminous intensity is *I* and the apparent area is *S'* (unit is m^2), the luminance *L* can be calculated by the following equation.    

> *L* = *I* / *S'*

The "apparent" unit area is the angle *Theta* that can be made in the line-of-sight direction to the normal of the light source or object surface, "*S'* = *S* * cos(*Theta*)".

![light_Luminance.jpg](./images/Lights/light_Luminance.jpg)     

For a diffuse reflective surface that is perfectly uniform for the angle of view (diffuse reflection distributed in a Lambertian hemisphere), the luminous intensity is "*I* * cos(*Theta*)" and the apparent area is "*S* * cos(*Theta*)",
In this case, the luminance does not change no matter which direction it is viewed from.     

Note that in the case of diffuse reflective surfaces or light distribution in the real world, luminous intensity will vary with angle.     
Therefore, luminance will vary depending on the angle of view.    

## Illuminance calculation

