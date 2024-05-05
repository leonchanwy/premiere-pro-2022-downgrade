# Premiere Pro Project Downgrader to 2022

This Apple Workflow automates the process of downgrading Premiere Pro project files (.prproj) from any version to be compatible with Premiere Pro 2022. This ensures that projects created with newer versions can be opened in Premiere Pro 2022, providing better version compatibility.

## Installation

1. Download the Automator Workflow file from this repository.
2. Double-click the downloaded file to install. The workflow will automatically integrate into your Finder's context menu.
3. You may need to confirm the installation by allowing it in your system preferences if prompted to do so.

## Usage

Once installed, you can use the workflow directly from the Finder using these simple steps:

1. Navigate to the Finder on your Mac and locate the .prproj files you wish to convert.
2. Select one or more .prproj files.
3. Right-click (or control-click) on the selected file(s) and choose the 'Downgrade to Premiere 2022' quick action from the context menu.
4. The workflow will process the files in place, modifying the version information to be compatible with Premiere Pro 2022.
5. Once the processing is complete, your files are ready to be opened directly in Premiere Pro 2022.

## How It Works

This Automator Workflow automates the following steps:

1. Decompresses the .prproj file, which is essentially a gzipped XML file.
2. Uses `sed` to search and replace the version number in the XML content, setting it to "40", which corresponds to the version compatible with Premiere Pro 2022.
3. Recompresses the modified XML back into a .prproj file, directly overwriting the original file.

## Safety Note

Before running this workflow, it is advisable to create backups of your original .prproj files. This script modifies the original files directly, and having backups ensures that you do not lose any data in case of unexpected issues.

## License

This project is open-sourced under the MIT License. See the `LICENSE` file for more details.
