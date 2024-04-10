# Photogrammetry-Processing-Automation-Tool
This Python script provides automation for various tasks related to photogrammetry. The script utilizes Pyside and Qt Designer for the graphical user interface. The GUI enables basic image processing for photogrammetry and exposes somne of Metashapes most commonly used parameters for scan processing. 

## Features

- **Load and Save Presets**: Allows users to load and save settings presets in JSON format.
- **Raw Image Processing**: Converts RAW image files (NEF format) to JPEG format with specified adjustments (exposure, shadows, highlights, sharpening).
- **Metashape Integration**: Automates the setup and execution of Metashape workflows based on user-defined parameters.
- **Project Folder Creation**: Generates project folder structures and copies necessary template files.

## Demo Video

[![Video Demo](https://img.youtube.com/vi/Jf9rVldZUv0/0.jpg)](https://www.youtube.com/watch?v=Jf9rVldZUv0)




## Directory Structure

project/

│

├── main.py           # Main script file

├── metashape.py      # Main script file

├── ui_mainwindow.ui  # Generated UI file (from Qt Designer)

├── ui_mainwindow.py  # UI design file 

├── resources.py      # resources for UI 

├── README.md         # Project documentation

├── LICENSE           # License file (if applicable)

├── requirements.txt  # Python dependencies

├── .gitignore        # Git ignore file

└─── other files and folders


## Dependencies

- Python 3.x
- `rawpy` library for RAW image processing, needed for Nikon .NEF processing
- `PIL` (Pillow) library for image processing
- `PySide6` library for Qt-based GUI
- `json` for JSON file handling

## Usage

1. **Installation**: Ensure Python 3.x is installed on your system.
2. **Install Dependencies**: Install required Python libraries using `pip`:
   ```bash
   pip install rawpy Pillow PySide6
   ```
3. **Run the Script**:
   - Execute the `main.py` script using Python:
     ```bash
     python main.py
     ```
4. **GUI Usage**:
   - Use the GUI to interact with different functionalities:
     - Click "Load" to load settings from a JSON preset file.
     - Adjust parameters using sliders and dropdowns.
     - Click "Save" to save current settings to a JSON preset file.
     - Click "Start" to initiate the automation process.
