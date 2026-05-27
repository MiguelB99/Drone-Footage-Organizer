# Drone Footage Organizer
A PowerShell script that automatically organizes DJI drone footage into folders by flight date.
## What It Does
- Scans a folder of unsorted drone files (videos and photos)
- Reads the actual flight date from DJI filenames (e.g., DJI_20251003155333_...)
- Moves each file into a dated folder like 2025-10-03_Flight
- Handles duplicate filenames automatically
- Logs every run to a text file
## Setup
1. Open OrganizeDroneFlights.ps1 in a text editor.
2. Update the three paths at the top to match your computer:
- $SourceFolder — where you copy files from your drone's SD card
- $DestinationFolder — where organized folders are saved
- $LogFile — where the activity log is written
## How to Run
1. Open PowerShell.
2. Navigate to the script's folder: cd C:\Scripts
3. First-time setup (only needed once): Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy RemoteSigned
4. Unblock the downloaded script: Unblock-File -Path .\OrganizeDroneFlights.ps1
5. Run the script: .\OrganizeDroneFlights.ps1
## Supported File Types
.mp4, .mov, .jpg, .dng, .raw
## Author
Miguel B — built as my first PowerShell project to organize drone footage.
