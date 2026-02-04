# ObjView

ObjView is a high-performance web-based viewer specifically designed for X-Plane OBJ8 files. It allows developers and artists to preview 3D models with full support for X-Plane's custom animation commands and material properties directly in the browser.

## Features

- **OBJ8 Support**: Native parsing of X-Plane OBJ8 files including vertex data, indices, and textures.
- **Animation Engine**: Full support for ANIM_trans, ANIM_rotate, ANIM_hide, and ANIM_show commands.
- **DataRef Simulation**: Interactive GUI to manipulate DataRefs and observe real-time animation behavior.
- **Advanced Materials**: Support for PBR workflows, including Albedo, Normal, and MAT (Metalness, Roughness, AO) maps.
- **View Modes**: Toggle between Material, Solid, Albedo, Roughness, Metallic, Lit Only, Normals, Wireframe, and Manipulators views.
- **Asset Management**: Drag and drop support for .obj, .png, .jpg, .bmp, .dds, and .hdr files.
- **Visibility Controls**: Manage complex scenes with object-level visibility toggles and solo modes.
- **Real-time Statistics**: Monitor vertex counts, triangle counts, and animation data for both individual selections and the entire scene.
- **Lighting & Environment**: Adjustable exposure, environment intensity, and rotation with HDR support.
- **ACF File Support**: Load X-Plane aircraft files (.acf) directly with full attached object parsing and positioning.
- **Livery System**: Automatic livery detection and switching with support for livery texture overrides.
- **VR Configuration**: Visualize VR teleport hotspots and preset views from _vrconfig.txt files.
- **Live Reload**: Automatic file monitoring with LIVE toggle for real-time updates during development.
- **Screenshot Tool**: Capture high-resolution screenshots with customizable backgrounds (solid, gradient, or transparent).
- **Tree View Organization**: Hierarchical folder structure for organizing complex scenes.
- **Manipulator Panel**: Detailed information panel showing DataRef paths, tooltips, and manipulator types.

## Keyboard Shortcuts

### General
- **F**: Recenter camera on the selected mesh or the entire scene.
- **Space**: Hold to temporarily override ANIM_hide and ANIM_show constraints (show all objects).
- **W/S**: Move camera forward/backward.
- **A/D**: Move camera left/right.
- **E/Q**: Move camera up/down.
- **Shift (hold)**: Move faster when using camera movement keys.

### Selection & Visibility
- **H**: Hide the currently selected mesh.
- **Shift + H**: Isolate selected meshes (toggle). Press again to restore previous visibility.
- **Alt + H**: Unhide all previously hidden meshes.
- **Shift + Click**: Select multiple meshes in the viewport.

### DataRef Sliders
- **Shift (Hold)**: Disable snapping to keyframe ticks when dragging sliders.
- **Double Click (DataRef Name)**: Copy the DataRef path to the clipboard.

### Shortcuts Overlay
- **?**: Open the keyboard shortcuts overlay.

## Mouse Controls

- **Left Click**: Select a mesh in the viewport.
- **Shift + Left Click**: Add/remove mesh from selection.
- **Right Click**: Unselect all meshes (when not dragging).
- **Right Click + Drag**: Orbit camera (default).
- **Middle Click + Drag**: Pan camera (default).
- **Scroll**: Zoom in/out.

## Technical Details

- **Rendering**: Three.js (WebGL 2.0)
- **Tone Mapping**: AgX
- **UI**: lil-gui for simulation controls
- **Texture Formats**: Support for standard image formats and DDS (via DDSLoader)
- **PBR Support**: MAT maps (Metalness/Roughness) and NORMAL_METALNESS workflows
- **Animation Interpolation**: Keyframe-based with snapping support
- **File System**: File System Access API for folder loading

## Usage

1. Open `obj8_webviewer.html` in a modern web browser (Chrome/Edge recommended).
2. Drag and drop .obj files, textures, or an entire aircraft folder.
3. Alternatively, click "Open ACF Folder" to load a complete X-Plane aircraft.
4. Use the DataRef sliders to test animations.
5. Toggle view modes to inspect materials and geometry.
6. Take screenshots with the screenshot tool for documentation.

<img width="2559" height="1270" alt="image" src="https://github.com/user-attachments/assets/44c611ef-047c-4829-994d-6217eb9b76ae" />
