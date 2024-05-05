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


# Premiere Pro 項目降級至2022版本

此Apple Workflow自動化了將Premiere Pro項目文件（.prproj）從任何版本降級以兼容Premiere Pro 2022的過程。這確保了用較新版本創建的項目可以在Premiere Pro 2022中打開，從而提供更好的版本兼容性。

## 安裝

1. 從本倉庫下載Automator Workflow文件。
2. 雙擊下載的文件進行安裝。該工作流將自動集成到您的Finder的右鍵菜單中。
3. 如果系統提示，您可能需要在系統偏好設置中確認安裝。

## 使用方法

安裝後，您可以直接在Finder中使用這些簡步驟使用工作流：

1. 在Mac的Finder中導航並定位到您希望轉換的.prproj文件。
2. 選擇一個或多個.prproj文件。
3. 右鍵（或控制點擊）所選文件，並從上下文菜單中選擇“降級至Premiere 2022”快速操作。
4. 工作流將就地處理文件，修改版本信息以兼容Premiere Pro 2022。
5. 處理完成後，您的文件即可直接在Premiere Pro 2022中打開。

## 工作原理

此Automator Workflow自動執行以下步驟：

1. 解壓.prproj文件，該文件本質上是一個gzipped的XML文件。
2. 使用`sed`命令在XML內容中搜索並替換版本號，將其設置為“40”，這與Premiere Pro 2022兼容的版本對應。
3. 將修改後的XML重新壓縮回.prproj文件，直接覆蓋原文件。

## 安全提示

在運行此工作流之前，建議創建您的原始.prproj文件的備份。此腳本直接修改原始文件，擁有備份可以確保在出現意外問題時不會丟失任何數據。

## 許可證

此項目在MIT許可證下開源。詳見`LICENSE`文件獲取更多詳情。