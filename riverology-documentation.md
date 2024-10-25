# Riverology Documentation

## Table of Contents
1. [Introduction](#introduction)
2. [Installation](#installation)
3. [Verification](#verification)
4. [Integration](#integration)
5. [Settings](#settings)
   - [Landscape](#landscape)
   - [Waves](#waves)
   - [Surface](#surface)
   - [Refraction](#refraction)
   - [Caustics](#caustics)
   - [Fog](#fog)
   - [God Rays](#god-rays)
   - [Debug](#debug)
6. [Buoyancy](#buoyancy)
7. [Spline Based Sound System](#spline-based-sound-system)
8. [Unreal Engine 5 Compatibility](#unreal-engine-5-compatibility)

## Introduction

Riverology is a mathematical wave simulation plugin for Unreal Engine, based on the Gerstner wave or trochoidal wave model. It's designed to describe the progression of waves on the surface of an incompressible fluid of infinite depth, making it suitable for deep-ocean wave simulations.Riverology leverages this technology to provide high-quality water simulations.

## Installation

1. Open the Epic Games Launcher and check which version of Riverology you need to install in your project.
2. Open your project in Unreal Engine.
3. Go to Settings -> Plugins -> River -> Riverology.
4. Enable the Riverology plugin.
5. In the Content Browser, select View Options -> Show Engine Content and Show Plugin Content.
6. Look for the folder called "Riverology_Plugin Content".

## Verification

To access private sections of the Riverology systems (documentation, video tutorials, support, etc.), you need to verify your ownership of the asset:

1. Leave a review or question on the UE4 marketplace page for Riverology.
2. Include your Discord Name in the message.
3. Join the Oceanology Community (link provided in the Discord).
4. Wait for manual verification. If not verified, contact @Developer Galidar or @zetxD.

After verification:

1. Find the "Important Code" channel in the Oceanology community Discord.
2. Copy the provided code.
3. Paste the code in your project's `DefaultEngine.ini` file (located at `Unreal Projects\YourProject\Config\DefaultEngine.ini`).

## Integration

To add Riverology to your map:

1. Create a new map with basic lighting.
2. In the Content Browser, navigate to Riverology_Plugin Content -> Advanced -> Blueprints -> Riverology.
3. Drag the Riverology asset into your map.

## Settings

### Landscape

- Apply Landscape Spline: Adapts the river to landscape heights.
- Raise Heights: Activates upward landscape deformation.
- Lower Heights: Activates downward landscape deformation.
- Deform Width: Modifies the deformation width.
- Deform Falloff: Controls the smoothness of deformation edges.

### Waves

Global Controls:
- Overall Length: Modifies wave length globally.
- Global Amplitude: Controls overall wave height.
- Global Speed: Adjusts wave speed globally.
- Choppiness: Creates more pronounced wave effects.

Custom Wave Controls:
- Amplitude: Customizes individual wave heights.
- Steepness: Increases wave sharpness.
- Wavelength: Modifies individual wave lengths.
- Direction: Controls wave direction.
- Direction Offset: Allows for complex directional control.

### Surface

- Surface Light Scattering: Controls light reflection and scattering.
- Anisotropy: Modifies light dispersion on the surface.
- Water Roughness: Adjusts surface roughness.
- Water Fresnel Roughness: Controls roughness at different distances.
- Water Specular: Manages light bounce intensity.
- Exponenth: Adjusts lighting intensity.
- Base Reflect Fraction In: Controls light refraction.

### Refraction

- Critical Angle Dot: Manages total internal refraction.
- Critical Angle Width: Controls reflection and refraction balance.
- Critical Angle Bend Width: Adjusts refraction angle at the surface.
- Refraction Bottom Amount: Alternative refraction method.
- Lip Refraction: Controls surface distortion.
- Refraction: Manages wave direction and speed in refraction.
- Refraction Far: Adjusts distant view refraction.
- Depth For Min Refraction: Sets minimum depth for surface refraction.

### Caustics

- Project Caustics: Enables caustics projection above the surface.
- Caustics Scale: Adjusts real-time caustics scale.
- Caustics Shore Mip: Controls caustics definition.
- Caustics Fade In Distance: Sets caustics depth at the surface.
- Caustics PlayBack FPS: Manages caustics animation speed.
- Caustics Velocity: Controls caustics movement speed.
- Caustics Brightness: Adjusts caustics intensity on the surface.

### Fog

- Enable Fog: Toggles Riverology's fog effect.
- Light Absorption: Controls light absorption in fog.
- Fog Scatter Color: Sets the main fog color.
- Fog Ambient Color: Adjusts ambient fog color.
- Absorption: Fine-tunes light absorption in fog.
- Band Color: Sets water cut effect color.
- Band Offset: Adjusts water cut height.
- Scattering Aniso: Controls skylight effect in fog.
- Wet Location: Sets head mist height.
- Wet Hardness: Increases water cut density.
- Wet Radius: Expands water cut radius.
- Band Opacity: Adjusts water cut opacity.
- Wet Alpha: Controls cut interpretation.
- Max Depth: Sets maximum fog density.

### God Rays

- Enable God Rays: Activates the god rays effect.
- Fog Ambient Color: Sets ambient mist color for god rays.
- Band Color: Adjusts water cut effect color in god rays.
- Wet Location: Controls head mist height for god rays.
- Wet Hardness: Increases cutting density of water in god rays.
- Wet Radius: Expands water cut radius in god rays.
- Max Depth: Sets maximum fog density for god rays.
- Band Opacity: Adjusts water cut opacity in god rays.
- Wet Alpha: Controls cut interpretation in god rays.

### Debug

- Draw Debug Line Width: Visualizes movement direction.
- Draw Debug Strings: Shows height location.
- Surface Debugging: Visualizes interaction with the spline.

## Buoyancy

To make an object float in Riverology:

1. Drag an object into your scene.
2. Set Mobility to Movable.
3. In the Physics category, enable Simulate Physics.
4. In the Physics Collision category, enable Generate Overlap Events.

Riverology's buoyancy system automatically determines the volume and density of objects.

## Spline Based Sound System

Riverology includes a sound-based spline system that can match deformations and curvatures in relation to sound.

## Unreal Engine 5 Compatibility

Riverology is compatible with Unreal Engine 5. For installation instructions specific to UE5:

1. Join the Oceanology community.
2. Complete the verification process.
3. Search for the UE5 installation tutorial in the community channels.

The latest version of Riverology includes a material system prepared for the most recent versions of Unreal Engine.

---

Thank you for being part of the Riverology adventure. Your support has been crucial in the development and success of this plugin. We're excited to bring you this update and grow our community.

Best regards,
The Oceanology Team
