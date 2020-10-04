ARCore-Depthmap-Enhancement

Directly Dealing with ARCore Depth API
=======================================
[depth lab](https://github.com/googlesamples/arcore-depth-lab/)

### Occlusion
Each pixel of the virtual object is tested whether it is located behind surfaces of the physical environment.
To reduce the blending artifacts, depth lab performs a soft blur in depth boundary regions

### Our Approach
**The bledning artifacts are not compeltely gone away even using blurring filter. Instead of blurring the boundary, we've decided to add graphic effect around the boundary. Users might feel more immersive and realistic rather than seeing awkward blurring effect near boundary regions. 

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
