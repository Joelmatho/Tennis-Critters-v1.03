# Tennis Critters v1.03 Decompiled

This repository contains the decompiled source code for **Tennis Critters v1.03**, a classic game originally released in 2007. The decompilation was performed using [DSO Sharp](https://github.com/Elletra/dso-sharp).

## Table of Contents

- [Common Issues](#common-issues)
  - [Flickering Shadows](#flickering-shadows)
  - [Audio Problems](#audio-problems)
- [Usage Instructions](#usage-instructions)
- [Acknowledgments](#acknowledgments)

## Common Issues

### Flickering Shadows

If you experience flickering shadows during gameplay, try replacing the `Opengl2d3d.dll` with a compatible version.

**Steps:**

1. **Download the DLL:** Get `Opengl32.dll` from [Mesa3D for Windows](https://github.com/lightningterror/Mesa3D-Windows).
2. **Replace the DLL:** Overwrite the existing `Opengl2d3d.dll` in your game directory with the downloaded `Opengl32.dll`.

### Audio Problems

Updating the OpenAL library can resolve certain audio issues.

**Steps:**

1. **Download OpenAL Soft:** Visit the [OpenAL Soft GitHub repository](https://github.com/kcat/openal-soft) for the latest version.
2. **Install OpenAL Soft:**
   - Extract the downloaded files.
   - Navigate to the `bin/Win32` directory.
   - Rename `soft_oal.dll` to `OpenAL32.dll`.
   - Place the renamed `OpenAL32.dll` in the same directory as the game’s executable.

**Note:**  
Some users have reported that this replacement may cause issues with certain audio formats (e.g., WAV files). If you encounter playback problems, revert to the original `OpenAL32.dll`. Contributions that address these issues are welcome via pull request.

## Usage Instructions

After applying any necessary fixes, launch the game by running its executable from the game directory.

## Acknowledgments

- **DSO Sharp:** The decompilation tool used to recover the source code. [GitHub Repository](https://github.com/Elletra/dso-sharp)
- **Mesa3D for Windows:** Provides the compatible OpenGL DLL. [GitHub Repository](https://github.com/lightningterror/Mesa3D-Windows)
- **OpenAL Soft:** The updated audio library. [GitHub Repository](https://github.com/kcat/openal-soft)

For further details and updates, please refer to the linked repositories.
