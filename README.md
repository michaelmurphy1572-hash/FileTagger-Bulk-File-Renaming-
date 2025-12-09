FileTagger User Guide

Overview

FileTagger is a standalone Windows application (.exe) for bulk-renaming files and flattening
folder structures. It is especially helpful for organizing large collections of photos, documents,
or any other files by adding consistent, customizable suffixes (e.g., year, custom text, folder
name, or sequential numbers).

• Author: Michael Murphy
• Version: Flex V1 (2024–2025)

The program requires no installation—just double-click the FileTagger.exe file to run it.
Getting Started

1. Double-click FileTagger.exe.
2. A brief splash screen with the program name will appear.
3. The application will quickly check for internet connectivity and updates (if a newer
version is available or there is no connection, a message will appear and the program
will close).
4. The main menu appears. Click Start to begin renaming files.
   
Main Window
1. Select Folder
• Click Browse… and choose the parent folder that contains the files you want to rename.
• All files in this folder and its subfolders will be processed (recursively).
2. Omit Subfolder from Renaming (optional)
• After selecting a folder, a dropdown lists its immediate subfolders.
• Select one to completely skip renaming any files inside that subfolder (and its own
subfolders).
3. Options
• Sequential Numbering (for suffix "Number") Checked = numbering continues across
all folders (0001, 0002, …). Unchecked = numbering restarts in each individual folder.
• Manual Year Selection (for suffix "Year") Check this box and enter a 4-digit year to
override the current year.
4. Suffix Slots (7 slots available)
Each slot can be enabled and set to exactly one of these types (they are mutually exclusive):
• Year – adds the current year or your manual year.
• Text – adds the custom text you type (invalid characters are replaced with underscores).
• Folder name – adds the name of the file’s immediate parent folder (leading numbers
and extra spaces are cleaned up).
• Number – adds a 4-digit sequential number (0001, 0002, …).
Enabled slots are applied from left to right (Suffix 1 → Suffix 7).
5. Preview
Displays exactly what the new suffix will look like (e.g., 2025_Client_Project_0001). Always
check this before proceeding.
6. Buttons
• Guide – opens a built-in help window.
• Save – saves your current configuration (suffixes, year, sequential setting, omitted
folder) to a settings file in your Documents folder. Settings load automatically the next
time you run the program.
• Continue – starts the renaming process.
• Undo – reverts the most recent rename operation (only the last batch).
• Sub Folder Removal – opens a separate tool for flattening folder structures (see below).
• Close – exits the program.
7. Log and Progress
While renaming, a real-time log shows each action (e.g., Renaming 'IMG_1234.jpg' to
'2025_Project_0001.jpg') and a progress bar indicates completion.

Sub Folder Removal Tool:
Click Sub Folder Removal (enabled after selecting a main folder).
Purpose:
Moves all files out of subfolders into a higher level and deletes the now-empty folders—perfect
for flattening deeply nested structures.

How to Use
1. Choose a top-level subfolder from the dropdown.
2. Select:
o Remove All Subfolders – flattens the entire structure under the chosen folder.
o Remove Lowest Level Sub Folders – only flattens the deepest level of folders.
3. Click Continue.
4. Files with the same name are automatically renamed with (1), (2), etc., to avoid
overwriting.
5. Use the Undo button in this window to completely reverse the operation (folders are
recreated and files moved back).

Undo Features
• Rename Undo – restores original filenames from the last rename operation only.
• Subfolder Removal Undo – recreates deleted folders and returns files to their original
locations.
• Undo works only for the most recent operation of each type and only if the files have not
been modified or moved by other programs afterward.

Tips
• Always verify the Preview before clicking Continue.
• Use Save after setting up your preferred suffix pattern—it will load automatically next
time.
• Avoid special characters (/\:*?"<>|) in custom text.
• The tool works with any file type.

Note the exact error message and send it to me with steps to reproduce.
