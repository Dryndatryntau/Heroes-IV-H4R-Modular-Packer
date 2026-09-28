========================================================================
            HEROES IV H4R MODULAR PACKER v1.0 (2026)
========================================================================

ABOUT THE PROGRAM
-----------------
"Heroes IV H4R Modular Packer" is a cross-platform, modular resource 
management tool designed for unpacking, packing, and editing "Heroes of 
Might and Magic IV" resource archives (.h4r) via plugins.

Available for both Windows (32-bit / 64-bit, including Windows XP)
and Linux operating systems.


KEY FEATURES & HIGHLIGHTS
-------------------------
1. H4R Archive Packer (Main Application):
   - Automatic RAW Format Conversion: When extracting raw audio 
     resources, the tool automatically splits and restores them into 
     standard .wav and .mp3 files, and converts "bitmap_raw" resources 
     into standard .bmp images, making them immediately usable in 
     external editors.
   - Archive Compatibility: Supports both .h4r archive versions (base 
     game and expansions), and packs new archives using the modern 
     expansion format (The Gathering Storm / Winds of War), which is 
     the standard used by the community today.
   - Resource Filtering & Extraction: Filter files by type (wav, mp3, 
     strings, tables, fonts, bitmaps, animations, etc.) and extract 
     all visible files or multi-selected items (Ctrl / Shift) into the 
     "unpacked" folder.
   - Archive Creation & Presets: Build new .h4r archives (saved to the 
     "packed" folder) with support for saving and loading file lists 
     via the "presets" folder.

2. Heroes IV Font Editor (Plugin "H4fnteditor"):
   - Complete viewer and editor for Heroes IV font (.fnt) files.
   - Import single characters or generate an entire font set from any 
     system-installed TrueType (TTF) font.
   - Supports multiple character encodings (Baltic CP1257, Western 
     CP1252, Central European CP1250, Cyrillic CP1251, etc.).
   - Built-in pixel-level glyph editor (4 grayscale levels, margin 
     adjustments, and Undo function).
   - Single or batch export/import of glyphs to/from .bmp files.
   - Automatically creates a .bak backup before overwriting .fnt files.

3. Centralized Localization & Modular Plugin System:
   - All UI strings for the main application and plugins are stored in 
     a single, centralized "lang/localization.ini" file. Each plugin 
     dynamically reads its translation from its respective section. 
     Adding a new language only requires translating the keys within this file.
   - Plugins (.dll on Windows, .so on Linux) are organized in subfolders 
     inside "plugins/" (e.g., "plugins/Heroes4/", "plugins/Heroes5/"). 
     The packer automatically scans all subfolders and dynamically 
     creates corresponding submenu branches under the "Plugins" menu.


IMPORTANT NOTE ON ANTIVIRUS SOFTWARE / PACKING (UPX)
----------------------------------------------------
Main executable files (.exe / Linux binaries) and Windows plugin 
libraries (.dll) are compressed using the UPX packer to reduce file size. 
Some Windows antivirus programs may flag UPX-compressed binaries as a 
false positive — the files are completely safe and clean.


TECHNICAL CREDITS & REFERENCES
------------------------------
- Open-source documentation on GitHub (AKuHAK) regarding the audio and 
  bitmap header structures, and the table layout concept from the "mh4" tool.
- Technical reference of the original .h4r Delphi unpacking engine logic 
  (M. Beschetnov / extractor.far.ru).
- Community research on the binary structure of Heroes IV fonts (.fnt).


AUTHOR & CONTACT
----------------
Author: Lapė Snapė
E-mail: dryndatryntau@gmail.com
Created: 2026
========================================================================
