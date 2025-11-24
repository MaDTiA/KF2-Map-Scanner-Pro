# KF2 Map Scanner Pro

A multi-threaded GUI application for Killing Floor 2 server administrators. Automatically scans directories for custom map files (KF-*.kfm) and generates the required .ini configuration blocks.

Features three switchable UI themes: Windows Native, Dark Professional, and Minimal Clean.

## Features

- Automated scanning: Recursively scans folders for .kfm map files
- Smart filtering: Identifies valid map files (KF-*.kfm pattern)
- INI generation: Creates formatted generated_maps.ini with required game flags
- Multi-threaded: Scanning runs in separate thread, UI stays responsive
- Live progress: Real-time progress bar and status updates
- Stop function: Safely interrupt scans in progress
- Theme switching: Three visual styles available at runtime
- DPI aware: Adjusts for high-resolution displays on Windows

## Requirements

Python 3.6 or higher. Uses only standard libraries (tkinter, os, threading).

## Installation

Clone or download this repository:

    git clone https://github.com/YOUR_USERNAME/KF2-Map-Scanner-Pro.git
    cd KF2-Map-Scanner-Pro

Run the script:

    python KF2-Map-Scanner-Pro.py

## Usage

1. Launch the application
2. Click "Browse KF2 Maps Folder" and select your maps directory
3. Optional: Click "Choose Output Location" to set custom save location
4. Select your preferred theme from the dropdown
5. Click "Start Scan" to begin
6. When complete, copy the generated .ini contents to your server's PCServer-KFGame.ini

## Output Format

Generated entries follow this structure:

    [KF-MapName KFMapSummary]
    MapName=KF-MapName
    MapAssociation=2
    ScreenshotPathName=UI_MapPreview_TEX.UI_MapPreview_Default
    bPlayableInSurvival=True
    bPlayableInWeekly=True
    bPlayableInVsSurvival=True
    bPlayableInEndless=True
    bPlayableInObjective=True

## Contributing

Pull requests are welcome. For major changes, open an issue first to discuss proposed changes.

## License

MIT License - see LICENSE file for details.

## Credits

Author: MaDTiA
Game: Killing Floor 2 by Tripwire Interactive
