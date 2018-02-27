# Godmode9 CIA Dumping and Building

### Dumping and Converting A Cartridge Game To CIA
1. Select [C:]GAMECART.
2. Select The [TitleID].trim.3ds file.
3. Select NCSD image options... > Build CIA from file.
4. The CIA will be in /gm9/out/titleid.cia (there may be more information than this in the name, that is perfectly fine and does not mean anything bad).

### Dumping An Installed SD Title As A CIA
1. Select [A:] SYSNAND SD.
2. Select title, highlight 00040000 if you are dumping a full title or 0004000e for an update, press R+A and select "Search for titles"
3. Find the title which you want to dump. The names are usually accurate enough.
3. Select TMD file options... > Build CIA (standard).
4. The CIA will be in /gm9/out/titleid.cia.

### Dumping A System Title As A CIA
*(Note: You may need the TitleID of the System App, a list of these can be found [here](https://www.3dbrew.org/wiki/Title_list "System Title List"))*
1. Select [1:] SYSNAND CTRNAND.
2. Highlight the title folder, press R+A and select "Search for titles"
3. Find the title which you want to dump. The names are usually accurate enough.
3. Select TMD file options... > Build CIA (legit).
4. The CIA will be in /gm9/out/titleid (+ the name and some other information).cia.
    - note: there may be something before .cia, it is perfectly fine.

### Dumping other files from CIAs (for ROM Hacking purposes)
1. Navigate to the .cia you wish to extract files from.
2. Select it and select CIA image options... > Mount image to drive.
3. Select the first folder, it should be called something like 0000.00000002 (names vary depending on the title).
    1. Make sure that the ROMFS is about the size of the installed title. If it is not, then the actual game content may be in another folder.
4. Select the files that you wish to extract.
    1. I.e. if you need a full romfs.bin, select that. .code (code.bin) is stored in the exefs folder.
    2. If you need specific game files, you can navigate through the romfs folder to find specific files.
5. Once you have either marked the files you want with L, and/or copied them with Y, hold R and press right on the d-pad to go to a new pane.
6. Navigate to a folder in which you wish to extract files to, and press Y to paste the files.

### Dumping other files from SD titles
1. Select [A:] SYSNAND SD.
2. Select title, highlight 00040000 if you are dumping a full title, 0004000e for an update press R+A and select "Search for titles"
3. Select the .tmd, and then "Open containing folder"
4. Select the largest .app > NCCH Options... > mount image to drive.
5. Select the files that you wish to extract.
    1. I.e. if you need a full romfs.bin, select that. .code (code.bin) is stored in the exefs folder.
    2. If you need specific game files, you can navigate through the romfs folder to find specific files.
6. Once you have either marked the files you want with L, and/or copied them with Y, hold R and press right on the d-pad to go to a new pane.
7. Navigate to a folder in which you wish to extract files to, and press Y to paste the files.

### Dumping other files from system titles
1. Select [1:] SYSNAND CTRNAND.
2. Highlight the "titles" folder, press R+A and select "Search for titles"
3. Select the .tmd, and then "Open containing folder"
4. Select the largest .app > NCCH Options... > mount image to drive.
5. Select the files that you wish to extract.
    1. I.e. if you need a full romfs.bin, select that. .code (code.bin) is stored in the exefs folder.
    2. If you need specific game files, you can navigate through the romfs folder to find specific files.
6. Once you have either marked the files you want with L, and/or copied them with Y, hold R and press right on the d-pad to go to a new pane.
7. Navigate to a folder in which you wish to extract files to, and press Y to paste the files.

### Dumping other files from a gamecart
1. Go to GAMECART > Titleid.3ds > NCSD image options... > mount image to drive.
2. Select content0.game (0 may be a different number).
3. Select the files that you wish to extract.
    1. I.e. if you need a full romfs.bin, select that. .code (code.bin) is stored in the exefs folder.
    2. If you need specific game files, you can navigate through the romfs folder to find specific files.
4. Once you have either marked the files you want with L, and/or copied them with Y, hold R and press right on the d-pad to go to a new pane.
5. Navigate to a folder in which you wish to extract files to, and press Y to paste the files.

### Dumping NCCH Images from a CIA for use with Citra (dlc titles will not work. As of like November builds, you can use updates with work)
1. Go to where the CIA is located, open it > CIA image options... > Decrypt file (...) > Decrypt inplace.
    1. You can choose to decrypt to 0:/gm9/out but you will need to navigate to the decrypted title.
    2. If it does fail, then the title is already decrypted and you can move on.
2. Open it again > CIA image options... > Mount image to drive.
3. You should see a folder (or two if the title has a manual) and .apps with the same names. Select the .app > NCCH image options... > decrypt file (0:/gm9/out).
    1. If you have multiple, go through each .app and make sure there is not a Manual.bcma inside of the romfs (the manual ncch image is typically around 3mb, so if you have another .app which is obviously larger, go with that one).
    2. If it does fail, then the title is already decrypted and you can move on. If it didn't fail, then you are done.
4. Select the same .app again and select Copy to 0:/gm9/out.
5. Rename the .app to have the file extension of .cxi.
6. Open in Citra and hope it doesn't crash (I don't know what to do if it does crash).
