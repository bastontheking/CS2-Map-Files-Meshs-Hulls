# CS2 Map Files (Meshs & Hulls)

## Overview

The `.baston` files in this repository are compressed JSON files used by the Baston.dev software to parse the mesh and hull data of maps. These files are optimized to be smaller in size!

## File Format

### Original JSON Files

Each map in originally consists of two JSON files:
- `mapName.json`: Contains the mesh data of the map.
- `mapName_hulls.json`: Contains the hull data of the map.

### Compressed

To reduce the file size and enhance security, the original JSON files are processed to create `.baston` files. This involves:
1. **Minification**: Removing all unnecessary whitespace and formatting from the JSON files.
2. **Compression**: Using GZIP to significantly reduce the file size.

The resulting files are named with the `.baston` extension:
- `mapName.baston`
- `mapName_hulls.baston`

## Purpose

The primary purposes of compressing and encrypting these files are:
- **Size Reduction**: To make the files smaller and easier for GitHub to accept and manage.

