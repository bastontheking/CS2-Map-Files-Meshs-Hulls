# CS2 Map Files (Meshs & Hulls)

## Overview

The `.baston` files in this repository are compressed and encrypted JSON files used by the Baston.dev software to parse the mesh and hull data of maps. These files are optimized to be smaller in size, making it easier for GitHub to accept them and for the software to load them efficiently.

## File Format

### Original JSON Files

Each map in originally consists of two JSON files:
- `mapName.json`: Contains the mesh data of the map.
- `mapName_hulls.json`: Contains the hull data of the map.

### Compressed and Encrypted Files

To reduce the file size and enhance security, the original JSON files are processed to create `.baston` files. This involves:
1. **Minification**: Removing all unnecessary whitespace and formatting from the JSON files.
2. **Compression**: Using GZIP to significantly reduce the file size.
3. **Encryption**: Using AES encryption to secure the data.

The resulting files are named with the `.baston` extension:
- `mapName.baston`
- `mapName_hulls.baston`

## Purpose

The primary purposes of compressing and encrypting these files are:
- **Size Reduction**: To make the files smaller and easier for GitHub to accept and manage.
- **Security**: To ensure that the data is secure and only accessible by authorized software and personnel.

## Usage in Baston.dev

The `.baston` files are used by the Baston.dev software to efficiently load and parse map data. The software is designed to handle the decryption and decompression of these files seamlessly, allowing for quick and secure access to the necessary map information.
