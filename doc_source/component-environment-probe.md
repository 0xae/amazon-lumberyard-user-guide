# Environment Probe<a name="component-environment-probe"></a>

Use the **Environment Probe** component to achieve the right visual quality for a space\. Environment probes help to determine proper reflections, ambient diffuse values, particle diffuse values, and shadow colors\.

For information about how to blend environment probes to create a smooth transition, for example, from day to night, see [Blending Environment Probes](level-blending-environment-probe.md)\.

The **Environment Probe** component has the following settings:

**Visible**  
Shows the light\.

**On initially**  
Specify if the light is on when created\.

## General Settings<a name="component-environment-probe-general-settings"></a>

See the following general settings:

**Color**  
The color of the light\.

**Diffuse multiplier**  
Sets the strength of the diffuse color\.

**Specular multiplier**  
Sets the strength of the specular brightness\.

## Environment Probe Settings<a name="component-environment-probe-settings"></a>

See the following environment probe settings:

**Area dimensions**  
The width, height, and depth in meters of the environment probe's effective area\.

**Sort priority**  
Priority number for probe rendering\. Lower priority numbers \(for example, **0** or **1**\) are rendered on top of the higher priority numbers \(for example, **100**\)\.

**Resolution**  
Cubemap resolution in pixels that is generated by this probe\.

**Box projected**  
Enables box projection\. Does not require regeneration of the cubemap\.

**Box height**  
Height of the box projection\.

**Box length**  
Length of the box projection\.

**Box width**  
Width of the box projection\.

**Attenuation falloff**  
The value that the light begins to falloff\. For example, a value or 1\.0 means the light starts to fall off at 1\.0 meter\. 

## Options<a name="component-environment-probe-options"></a>

See the following options:

**View distance multiplier**  
Adjusts the maximum view distance\. For example, **1\.0** uses the default and **1\.1** is 10% farther than the default\.

**Minimum spec**  
Minimum specification value at which the light is enabled\.

**Voxel GI mode**  
Mode for light interaction with voxel global illumination \(GI\)\.

**Use VisArea**  
Light is affected by visible areas\.

**Indoor only**  
Light is only rendered indoors\.

**Affects this area only**  
Light affects only the immediate area\.

**Volumetric fog only**  
Light affects only volumetric fog\.

**Volumetric fog**  
Light affects volumetric fog and surrounding area\.

## Animation<a name="component-environment-probe-animation"></a>

See the following animation settings:

**Style**  
Enter a number to specify a preset light animation curve to play as defined in the `Light.cfx` file\. Valid values are **0** to **48**\. You can also use values **40** to **48** for testing and debugging\.

**Speed**  
Multiple of the base animation rate\. For example, a value of **2\.0** makes an animation play twice as fast\.

**Phase**  
Animation start offset from **0** to **1**\. A value of **0\.1** is 10% into the animation\. For example, you can use this setting to prevent lights in the same scene, with the same animation, from being animated in unison\.

## Cubemap Generation<a name="component-environment-probe-cubemap"></a>

See the following cubemap generation settings:

**Cubemap**  
Click **Generate** to generate or regenerate a cubemap for this probe\. The button is enabled only when **Use customized cubemap** is deselected\.  
Click **Reset** to reset a cubemap for this probe\.

**View cubemap**  
Displays a preview of the cubemap in the viewport\. You can only select this option when a cubemap exists\.

**Use customized cubemap**  
If selected, you can specify a custom cubemap for **Cubemap asset**\. If deselected, a cubemap is generated\.

**Cubemap asset **  
File path for the cubemap asset\.

## Additional Resources<a name="component-environment-probe-additional-links"></a>

For more information about the **Environment Probe** component, see the following:
+ [Intro to Environment Lighting](https://docs.aws.amazon.com/lumberyard/latest/userguide/enviro-lighting-intro.html) 
+ [Getting Started: Using Lighting Tutorial \(video\)](https://www.youtube.com/watch?v=-KdwKZtzzo0)

## EBus Request Bus Interface<a name="component-environment-probe-ebusrequest"></a>

Use the following request functions with the EBus interface to communicate with other components of your game\.

For more information about using the event bus \(EBus\) interface, see [Working with the Event Bus \(EBus\) system](ebus-intro.md)\.

All light components share common EBus functions\. For more information, see [Light Components EBus Request Bus Interface](component-area-light.md#component-light-ebusrequest)\.