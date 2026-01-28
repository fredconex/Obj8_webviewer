# ObjView

ObjView is a high-performance web-based viewer specifically designed for X-Plane OBJ8 files. It allows developers and artists to preview 3D models with full support for X-Plane's custom animation commands and material properties directly in the browser.

## Features

- OBJ8 Support: Native parsing of X-Plane OBJ8 files including vertex data, indices, and textures.
- Animation Engine: Full support for ANIM_trans, ANIM_rotate, ANIM_hide, and ANIM_show commands.
- DataRef Simulation: Interactive GUI to manipulate DataRefs and observe real-time animation behavior.
- Advanced Materials: Support for PBR workflows, including Albedo, Normal, and MAT (Metalness, Roughness, AO) maps.
- View Modes: Toggle between Material, Solid, Albedo, Lit Only, Normals, and Wireframe views.
- Asset Management: Drag and drop support for .obj, .png, .jpg, .bmp, .dds, and .hdr files.
- Visibility Controls: Manage complex scenes with object-level visibility toggles and solo modes.
- Real-time Statistics: Monitor vertex counts, triangle counts, and animation data for both individual selections and the entire scene.
- Lighting & Environment: Adjustable exposure, environment intensity, and rotation with HDR support.

## Keyboard Shortcuts

### General
- F: Recenter camera on the selected mesh or the entire scene.
- Space: Hold to temporarily override ANIM_hide and ANIM_show constraints (show all objects).

### Selection & Visibility
- H: Hide the currently selected mesh.
- Shift + H: Unhide all previously hidden meshes.
- Shift + Click: Select multiple meshes in the viewport.

### DataRef Sliders
- Shift (Hold): Disable snapping to keyframe ticks when dragging sliders.
- Double Click (DataRef Name): Copy the DataRef path to the clipboard.

## Technical Details

- Rendering: Three.js (WebGL 2.0)
- Tone Mapping: AgX
- UI: lil-gui for simulation controls
- Texture Formats: Support for standard image formats and DDS (via DDSLoader)

<img width="2559" height="1270" alt="image" src="https://github.com/user-attachments/assets/44c611ef-047c-4829-994d-6217eb9b76ae" />
