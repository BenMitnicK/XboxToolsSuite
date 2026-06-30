# XboxToolsSuite V2

XboxToolsSuite V2 is a modern toolkit for working with original Xbox resource files, textures, and meshes.

## Features

### Main Application

- Tab-based layout:
  - XIP Tools
  - XBX Tools
  - XMTools and Bios BOOT
  - Options
- Modern OpenGL mesh preview
- Transparent splash screen support
- Selectable splash screen logo
- Optional non-transparent splash screen frame
- Application reboot action from the File menu

### XIP Tools

XIP Tools is used to inspect, edit, create, and extract Xbox XIP archives.

Features:

- Open one or multiple `.xip` archives
- Create new XIP archives
- Save current archive
- Save all modified archives
- Drag and drop `.xip` files into the application
- Add files into an archive
- Replace existing files with confirmation
- Delete selected entries
- Rename entries
- Extract selected entries
- Extract all entries
- Search/filter entries inside an archive
- Show or hide internal buffers
- Multiple XIP tabs
- Right-click menu on XIP tabs:
  - Save As
  - Close
  - Close Others
  - Close All
- Custom Xbox file icons for:
  - XIP
  - XBX texture
  - XM mesh
  - XAP
  - Audio
  - Generic files
- XBX texture preview directly from a XIP archive
- XM mesh preview directly from a XIP archive through the XMTools tab

### XBX Tools

XBX Tools converts Xbox texture files and common image files.

Conversion modes:

- IMG -> XBX
- XBX -> PNG
- ALL

IMG -> XBX:

- Supported input formats:
  - PNG
  - JPG
  - JPEG
  - BMP
- Native DXT3 XBX/XPR output
- Fast quality mode
- High quality mode
- Power-of-two size validation
- DXT block size validation

XBX -> PNG:

- Supported input formats:
  - `.xbx`
  - `.xpr`
- Supported texture formats:
  - DXT1
  - DXT2 / DXT3
  - DXT4 / DXT5
  - A8R8G8B8
  - X8R8G8B8
- Swizzled ARGB decoding
- PNG output

Tools:

- Convert
- Clear Log
- Open Input Folder
- Open Output Folder
- Optional output cleanup before conversion
- Conversion log / progress console
- Automatic default folders:
  - `img2xbx_IMG`
  - `img2xbx_XBX`
  - `xbx2png_XBX`
  - `xbx2png_PNG`

### XMTools

XMTools handles Xbox `.xm`, DirectX `.x`, and Wavefront `.obj` mesh files.

Supported mesh formats:

- Xbox Mesh `.xm`
- DirectX Mesh `.x`
- Wavefront OBJ `.obj`

Mesh Tools features:

- Open `.xm`, `.x`, `.obj`
- Preview meshes with modern OpenGL
- View modes:
  - Total View
  - Solid Shaded Optimized
  - Realistic Shaded
  - Wireframe
- Convert `.x` to `.xm`
- Convert `.xm` to `.x`
- Convert `.obj` to `.xm` or `.x`
- Batch convert:
  - `.x` -> `.xm`
  - `.xm` -> `.x`
- Export current mesh as OBJ
- Open OBJ in the integrated OBJ Editor tab
- Mesh information tree:
  - File source
  - Polygons
  - Vertices
  - Indices
  - FVF
  - Stride
  - Bounding box
  - Mesh size
  - Center
  - Bounding sphere
  - Vertex format
  - Vertex buffer layout
  - Index buffer
  - Mesh statistics
  - Texture coordinates
  - Face analysis
- Mesh context menu:
  - Set Mesh FVF
  - Center Mesh
  - Reset Transform
  - Scale x0.5
  - Scale x2
- Keyboard movement in Mesh Tools:
  - Arrow keys: move mesh on X/Y
  - Z + Up/Down: move mesh on Z

### OBJ Editor

The OBJ Editor is integrated as an XMTools sub-tab. It is an editor, not a standalone viewer.

Features:

- Open OBJ mesh
- Keep the original object origin/pivot when opening
- Reset object to original imported state
- Center Auto to center the object on the grid
- Scale from programmed target
- Scale from a reference mesh
- Scale x0.5
- Scale x2
- Save edited object as `.x`
- Save edited object as `.xm`
- Non-destructive transform state until export/save
- Modern OpenGL grid and object rendering
- Help panel with icons

OBJ Editor controls:

Navigation:

- Left mouse drag: move object on X/Z grid
- Right mouse drag: rotate full view
- Ctrl + left mouse drag: pan full view
- Mouse wheel: camera zoom
- X + mouse wheel: scale object
- X + Left/Right: scale object down/up

Movement:

- Arrow keys held: continuous movement on X/Z
- Y + Up/Down: move object on Y

Rotation:

- M + Left/Right: rotate object X
- M + Up/Down: rotate object Y
- Z + Left/Right: rotate object Z

View:

- R: reset transform
- V or Home: high diagonal view

Scale:

- 1: scale x0.5
- 2: scale x2

Save and Help:

- F5: save `.x`
- F6: save `.xm`
- H: show/hide help

### Options

SplashScreen options:

- Select splash logo:
  - XboxToolsSuite 1
  - XboxToolsSuite 2
  - XboxToolsSuite 3
  - XboxToolsSuite 4
  - XboxToolsSuite 5
- Transparency:
  - Transparent Logo
  - No Transparency
- Resize logo to fit splash

XIP Tools options:

- Add Files:
  - Show only `.xap`, `.xm`, and `.xbx`

XMTools options:

- Mesh import:
  - Open OBJ/X files without Xbox XM vertex limit
- XM limit:
  - Offer automatic vertex welding when saving oversized XM
- Reference overlay color:
  - Choose the color used for the reference overlay in the Object Editor

Toolbar Icons options:

- XIP Tools icon size:
  - 32, 48, 64, 80, 96, 110, 128
- XBX Tools icon size:
  - 32, 48, 64, 80, 96, 110, 128
- XMTools icon size:
  - 32, 48, 64, 80, 96, 110, 128
- Object Editor icon size:
  - 32, 48, 64, 80, 96, 110, 128

## ScreenShots

<img width="1222" height="852" alt="XIPTools" src="https://github.com/user-attachments/assets/d7ae4961-4d68-4a89-8f16-5e4f5f137005" />
<img width="1222" height="852" alt="XBXTools" src="https://github.com/user-attachments/assets/0a26960a-cfce-40b9-b0b4-dff30cee521a" />
<img width="1222" height="852" alt="XMTools" src="https://github.com/user-attachments/assets/364c44d1-3296-48a8-b648-c9b0178fd377" />
<img width="1222" height="852" alt="EditorObject" src="https://github.com/user-attachments/assets/2374ca6d-766f-410f-ad33-3baaa834fbf5" />
<img width="1222" height="852" alt="optionbs" src="https://github.com/user-attachments/assets/e6cf3cc0-7099-478c-8d40-472c6250ad11" />

[![Watch the video](https://img.youtube.com/vi/SMgHC59NoNs/hqdefault.jpg)](https://www.youtube.com/watch?v=SMgHC59NoNs)
