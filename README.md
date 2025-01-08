# Tennis Critters v1.03 Decompiled

This repository contains the decompiled source code for **Tennis Critters v1.03**, a classic game originally released in 2007. The decompilation was achieved using the [DSO Sharp](https://github.com/Elletra/dso-sharp) tool.

## Decompilation Tool

The decompilation was performed using [DSO Sharp](https://github.com/Elletra/dso-sharp), a DSO decompiler for the Torque Game Engine. It converts `.dso` files back into TorqueScript, facilitating analysis and modification.

## Resolving Common Issues

### Flickering Shadows

If you experience flickering shadows during gameplay, replacing the `Opengl32.dll` file with a compatible version can help.

1. **Download the DLL**: Obtain the `Opengl32.dll` from [Mesa3D for Windows]([https://github.com/lightningterror/Mesa3D-Windows]).
2. **Replace the DLL**: Replace `Opengl2d3d.dll` with the downloaded `Opengl32.dll`.

### Audio Issues

To address audio problems, updating the OpenAL library can be beneficial.

1. **Download OpenAL Soft**: Visit the [OpenAL Soft GitHub repository](https://github.com/kcat/openal-soft) to download the latest version.
2. **Install OpenAL Soft**:
   - Extract the downloaded files.
   - Navigate to the `bin` directory.
   - then Navigate to the `Win32` directory.
   - Rename `soft_oal.dll` to `OpenAL32.dll`.
   - Place the renamed `OpenAL32.dll` in the same directory as the game's executable file.

**Important Note**: Some users have reported that replacing the `OpenAL32.dll` with OpenAL Soft's version can cause issues with certain audio formats, such as WAV files. If you experience audio playback problems after updating to OpenAL Soft, consider reverting to the original `OpenAL32.dll` provided with the game. **If you find a fix, please make a pull request.**

## Acknowledgments

- [DSO Sharp](https://github.com/Elletra/dso-sharp) for the decompilation tool.
- [Mesa3D for Windows](https://fdossena.com/?p=mesa%2Findex.frag) for the OpenGL DLL.
- [OpenAL Soft](https://github.com/kcat/openal-soft) for the audio library.

For further information and updates, please refer to the respective repositories linked above. 
