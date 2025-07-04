# Custom Debloated Blox Launcher (CDBL)

**Custom Debloated Blox Launcher (CDBL)** is a Windows utility for customizing and managing your Roblox installation.  
It allows you to easily patch, restore, and personalize Roblox with custom skyboxes, dark textures, and more—all with a user-friendly interface.

Use [THIS](https://github.com/eman225511/Auto-Install-Skybox-and-Dark-Textures/releases/download/updare/Old-CLI.zip) if you have issues (its an old version)

[Virustotal](https://www.virustotal.com/gui/url/79bdafe673df56a870093405b180b1d03b61f9e1bc4e49add6ee366be3329a85)

[Install Guide](https://github.com/eman225511/CustomDebloatedBloxLauncher?tab=readme-ov-file#installation--usage)

---

## Features

- **Skybox Manager:**  
  Browse, preview, and apply a wide selection of custom skyboxes. Skyboxes are downloaded on demand and stored in `%LOCALAPPDATA%\CustomBloxLauncher\Skyboxes`.

- **Skybox Previews:**  
  All skybox previews are downloaded and extracted from a single ZIP, stored in `%LOCALAPPDATA%\CustomBloxLauncher\Previews`.

- **Dark/Light/Default Textures:**  
  Easily switch between dark, light, and default Roblox textures.

- **Settings Tweaks:**  
  Adjust sensitivity, FPS cap, graphics, and volume using a PowerShell script.

- **Restore Functions:**  
  Restore original Roblox skyboxes and textures at any time.

- **Automatic Dependency Handling:**  
  The included `Install-and-Run.bat` script will install Python 3.12 (if needed), set up dependencies, and launch the app—even if your folder has spaces.


|   |  |
| ------------- | ------------- |
| ![alt](Preview3.png)  | ![alt](Preview1.png)  |
| ![alt](Preview4.png)  | ![alt](Preview2.png)  |

---

## Installation & Usage

1. **Go to [Here](https://github.com/eman225511/CustomDebloatedBloxLauncher/releases/latest) and downlaod `CDBL.zip`**

2. **Run the Launcher Script**

   Double-click `Install-and-Run.bat`.  
   - This will install Python 3.12 (if needed), dependencies, and launch the app as administrator.

3. **Using the App**

   - **Skyboxes:**  
     Select a skybox from the list to preview. Click "Apply" to download and install it.
     - for custom use this [Guide](CustomSky.md)
   - **Textures:**  
     Use the buttons to apply dark, light, or default textures.
   - **Settings:**  
     Use the settings dialog to tweak Roblox settings.
   - **Restore:**  
     Use the restore options to revert to original Roblox files.

---

## File Structure Of Github

```
CDBL/
│
├─ main.py                # Main application code
├─ Install-and-Run.bat    # One-click installer and launcher
├─ requirements.txt       # Python dependencies
├─ src/
│   ├─ DarkTextures/      # Dark textures directory
│   ├─ DarkTextures.zip   # Dark textures ZIP archive
│   ├─ DefaultSky/        # Default skybox directory
│   ├─ DefaultSky.zip     # Default skybox ZIP archive
│   ├─ DefaultTextures/   # Default textures directory
│   ├─ DefaultTextures.zip# Default textures ZIP archive
│   ├─ LightTextures/     # Light textures directory
│   ├─ LightTextures.zip  # Light textures ZIP archive
│   ├─ SkyboxPNGs/        # Skybox PNG images
│   ├─ SkyboxPatch/       # Skybox patch directory
│   ├─ SkyboxPatch.zip    # Skybox patch ZIP archive
│   ├─ SkyboxZIPs/        # Skybox ZIPs storage
│   └─ skybox/            # (Legacy) Local skybox storage (now uses %LOCALAPPDATA%)
├─ func/
│   ├─ APIFunc.py         # Download, unzip, and utility functions
│   ├─ ApplySkybox.py     # Skybox patching logic
│   ├─ ApplyDark.py       # Dark texture patching logic
│   ├─ ChangeSettings.ps1 # PowerShell settings script
│   ├─ GlobalBasicSettings_13.xml # Settings XML
│   ├─ Restore.py         # Restore functions
│   └─ __pycache__/       # Python bytecode cache
└─ README.md
```

---

## Data Storage

- **Skyboxes:**  
  `%LOCALAPPDATA%\CustomBloxLauncher\Skyboxes\`

- **Skybox Previews:**  
  `%LOCALAPPDATA%\CustomBloxLauncher\Previews\`

- **Downloads (temp):**  
  `%LOCALAPPDATA%\CustomBloxLauncher\Downloads\`

---

## Requirements

- Windows 10/11
- Python 3.12 (auto-installed if missing)
- Internet connection (for downloading skyboxes, previews, and patches)

---

## Credits

- Mega thanks to [fleasion/Fleasion](https://github.com/fleasion/Fleasion) for the method 
- [KickfnGIT/DebloatedBloxLauncher](https://github.com/KickfnGIT/DebloatedBloxLauncher) for this [code](https://github.com/eman225511/CustomDebloatedBloxLauncher/blob/main/func/ChangeSettings.ps1)
- Huge thanks to @kaizenken on discord for the skyboxes
- And huge thanks to @alana.py on discord for the help
- Github copilot for UI and Readme

---

## License

This project is for educational and personal use.  
Not affiliated with Roblox Corporation.
