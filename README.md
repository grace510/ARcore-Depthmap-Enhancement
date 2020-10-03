ARCore-Depthmap-Enhancement

Directly Dealing with ARCore Depth API
=======================================
[depth lab](https://github.com/googlesamples/arcore-depth-lab/)

### Three different ways to access depth
1. Localized depth: Sample single depth values at certain texture coordinates (CPU)
2. Surface depth: Create a connected mesh representation of the depth data (CPU/GPU)
3. Dense depth: Process depth data at every screen pixel (GPU)


### Shader
[Occlusion Effect Shader](https://github.com/google-ar/arcore-unity-sdk/blob/master/Assets/GoogleARCore/Examples/Common/Materials/Shaders/OcclusionImageEffect.shader)

[Camera Color Ramp Shader](https://github.com/google-ar/arcore-unity-sdk/blob/master/Assets/GoogleARCore/Examples/Common/Materials/Shaders/CameraColorRampShader.shader)



CNN for Denoising Depth Noise
=======================================
Noised Image Input Dataset: Created by adding [Kinect Simulated Noise](https://github.com/ankurhanda/simkinect) to [NYU2 depth dataset](https://drive.google.com/file/d/1WoOZOBpOWfmwe7bknWS5PMUCLBPFKTOw/view)
