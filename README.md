![preview](https://raw.githubusercontent.com/puffballz112742-ctrl/mhworld-rig-utilities/main/poster_a8640.svg)

# VoxelForge: Monster Hunter World — Realtime Mesh Studio

**Where low-poly meets high-fidelity.** VoxelForge is a groundbreaking Blender addon that transforms Monster Hunter World's dense, high-resolution 3D assets into fully-editable, lightweight voxel representations — all within a single seamless workflow. Instead of simply importing raw model files, this suite bridges the gap between the game's complex geometry and the artist's need for clean, modular, and performance-friendly building blocks.

Whether you are a technical artist, a game modder, or a hobbyist recreating the New World, VoxelForge empowers you to deconstruct, rebuild, and reimagine the intricate armor, weapons, and endemic life of Monster Hunter World without getting lost in a swamp of polygon soup. This is not just an importer; it is a **geometric translation engine** designed to turn dense data into a creative sandbox.

## Overview

The traditional approach to handling game assets involves importing massive, unoptimized meshes directly into your scene, often leading to viewport lag and a nightmare of non-destructive editing. VoxelForge flips this paradigm by performing a smart **voxelization pass** during the import process.

Instead of dealing with millions of triangles, you receive a clean, volumetric grid of "cubes" that perfectly encapsulates the silhouette and surface detail of the original asset. This allows for unprecedented flexibility: you can easily sculpt, paint, or apply physics simulations to these voxel clusters as if they were raw clay, all while maintaining the iconic identity of the original Monster Hunter designs.

Our addon is built for the 2026 pipeline, ensuring compatibility with the latest Blender LTS releases and the modern hardware acceleration features that make real-time voxel manipulation possible. We focus on **user empowerment** and **data fidelity**, ensuring that every Rathalos scale and Nergigante spike is represented accurately in this new dimensional format.

## [![Download](https://raw.githubusercontent.com/puffballz112742-ctrl/mhworld-rig-utilities/main/btn_091b365.svg)](https://puffballz112742-ctrl.github.io/mhworld-rig-utilities/)

## Why VoxelForge? The Core Philosophy 💡

Imagine trying to read a novel where every word is a block of granite. That is what traditional high-poly importing feels like. VoxelForge turns those granite blocks into a bag of building blocks. Here is why this matters:

- **Sacrifice Nothing, Gain Everything:** While we reduce geometric complexity, we retain the **normal map data** and **vertex color information** during the voxelization process. This means your voxel models look surprisingly detailed, despite being built from cubes.
- **Physics-Ready Topology:** Voxel grids are the perfect foundation for particle simulations, soft-body dynamics, and destruction effects. Drop a voxelized Great Sword, and watch it shatter into discrete, weighty chunks in real time.
- **A True Neutral File Format:** The output is not a proprietary Blender-only format. You can export your voxel sculptures to `.vox`, `.gltf`, or even `.obj` for use in game engines, 3D printing, or other DCC tools.
- **The Anti-Tessellation Engine:** We don't just reduce vertex count; we **restructure intent**. You see the volume, not the surface. This unique perspective often leads to new creative solutions, like building custom weapons from the "inside out."

## Featured Capabilities: The Tool Suite 🛠️

This suite is not a single command; it is a curated collection of utilities designed to handle every stage of the voxel transformation process.

- **⛏️ Smart Variant Importer:** Automatically detects monster species, weapon subtypes, and armor variations. The importer reads the file structure to distinguish between high-poly "Zorah" versions and standard models.
- **📦 Mesh-to-Voxel Converter:** The core engine. Offers granular control over **resolution (voxel size)**, **hollowing**, and **surface gap tolerance** .
- **🔨 Boolean Sculpting Kit:** Post-import tools to add or subtract voxels using custom brush shapes, allowing you to fuse a Rathian wing with a Uragaan shell.
- **🏷️ UV & Material Retopology:** Automatically remaps the original PBR textures onto the voxel grid faces, ensuring your materials don't break when you convert.
- **🖥️ Responsive 24/7 Processing:** The addon's core code is designed to run asynchronously. You can keep working on other parts of your scene while the voxelization process churns through data in the background, maximizing your workflow efficiency.
- **🌐 Multilingual UI Control:** The interface responds dynamically to your Blender language settings, supporting English, Japanese, Korean, and German to serve the global Monster Hunter community.

## Getting Started: From Zero to Voxel Hero 🚀

This section is your launchpad. We assume you have a basic understanding of Blender, but even if you are a newcomer, the process is intuitive.

### Step 1: Acquisition & Setup

To obtain VoxelForge, please use the download link provided above. After downloading, install the addon via Blender's **Edit > Preferences > Add-ons > Install...** function. Ensure you enable it by ticking the checkbox next to "Import-Export: VoxelForge Suite."

### Step 2: Preparing Your First Asset

1.  Navigate to **File > Import > Monster Hunter World (Voxel)** .
2.  Select a file with the `.mod3` or `.gmd` extension.
3.  In the Operator Panel (bottom left of the viewport), you will see a new category: **Voxel Baking Options**.
4.  Set the `Voxel Resolution` to 0.05 for a balance between detail and performance, or lower it to 0.01 for maximum fidelity.

### Step 3: The Transformation

Click **Import Voxelized**. The addon will read the mesh data, perform the conversion, and drop a new object named `VX_` + `AssetName` into your collection. The original material slots are preserved, and a new Geometry Node setup is automatically attached to allow for parametric edits.

### Step 4: Exporting or Editing

You are now free to:
- Sculpt the voxel cloud using standard Blender sculpting brushes (with Dyntopo enabled).
- Apply a **Boolean Union** modifier to voxelize multiple objects together.
- Export to `.vox` via our dedicated exporter under the same menu.

## System Requirements & Compatibility 🖥️

- **Blender:** Versions 4.0 LTS and later (Optimized for 4.5+ and the 2026 release cycle).
- **Operating System:** Windows 10/11, macOS 13+, Linux (x86_64).
- **Hardware:** A minimum of 8 GB RAM is required. 16 GB is recommended for large monster files. A dedicated GPU with 4GB VRAM is recommended for real-time viewport previews.

## The Technical Edge: How We Differ 📊

| Feature | Traditional Importers | VoxelForge Suite |
| :--- | :--- | :--- |
| **Output Geometry** | High-poly N-gons | Uniform Voxel Cubes |
| **File Size (Blender)** | Large (50-100 MB) | Lightweight (5-15 MB) |
| **Physics Suitability** | Poor (Complex collisions) | Excellent (Primitive shapes) |
| **Editability** | Hard Surface Booleans | Dynamic Volume Sculpting |
| **Data Retention** | Full UV & Normal Maps | Compressed, Tileable Textures |

## Empowering Your Workflow: The Ecosystem

We understand that tools are only as good as their integration. VoxelForge offers an **Open Bridge API** for developers who wish to write custom exporters to game engines or specialized rendering software. This allows for a unique level of automation, ensuring that your voxel creations can travel beyond Blender.

Furthermore, our **community-driven preset libraries** allow you to save and share specific voxel configurations (e.g., "High-Poly Wyvern Print," "Low-Poly Decor Base"). This ensures consistency across large projects and teams.

## License & Legal Disclaimer 📜

VoxelForge is an independent project and is **not affiliated with Capcom** or any of its subsidiaries. All asset names, monster titles, and in-game references are used solely for identification purposes and remain the property of their respective owners.

The conversion process is transformative, creating new, functional data structures. This tool is distributed under the **MIT License**, allowing you to modify and redistribute the code under the terms of that license.

### MIT License

Copyright (c) 2026 VoxelForge Project

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

## Limitations & Fair Use Notice

This tool is intended for **educational purposes, game modding, and artistic study**. It is not intended for commercial redistribution of Capcom's original assets or textures. The voxelization process creates derivative data, but we encourage users to respect the intellectual property of the original creators. If you intend to use voxel assets in a commercial project, we strongly advise you to create substantial changes to the geometry and textures to ensure your work constitutes a **transformative use.**

We prioritize transparency: this suite does not connect to any online servers, tracking services, or data-mining operations. All processing is done locally on your machine, ensuring your privacy and security.

## Join the Future of Mesh Handling

VoxelForge is more than just a modification tool; it is a new way of looking at dense 3D data. We invite you to break the mold and build something unique from the ashes of high-poly complexity. The final key to unlocking your creative potential is just a click away.

## [![Download](https://raw.githubusercontent.com/puffballz112742-ctrl/mhworld-rig-utilities/main/btn_091b365.svg)](https://puffballz112742-ctrl.github.io/mhworld-rig-utilities/)