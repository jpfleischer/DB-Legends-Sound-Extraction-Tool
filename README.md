# DB-Legends-Sound-Extraction-Tool
Tool to extract sound files from Dragon Ball Legends (mobile game). Windows only.

You need vgmstream-cli from https://vgmstream.org/ (command-line). Put the contents in a folder named "vgmstream-cli" next to the exe.

Steps: 

1 - Rename all files in the streamingassetbundles folder to have the .acb extension. (A batch file to number them and append the extension will be included)

2 - Run the exe. The tool will sort all possible files based on their contents and create a .bat file to extract them. 

3 - Extract sorted files through the console or by clicking on the generated batch files. 

4 - For files that weren't sorted or named correctly, you can check contents manually by opening the .acb file with notepad, but you can still extract them. 

5 - You can then freely delete all .acb files that were extracted. You'll have to delete them manually for the ones that weren't.

The streamingassetbundles folder includes assets, movies and sound files of types I couldn't extract, they'll be put in the right folder as needed.

Very Specific Notes: 
- The tool sorts the files based on the description inside inside the packages, it highly depends on the devs using consistent naming patterns, avoiding mistakes and keeping them separated, and thus it's far from perfect. Extracting the files shows their individual content in their name and should make it easier.  
- There are very few cases of the sort not working correctly (not using the character name) that I chose to ignore due to their infrequency. As for files that fail to sort, there are currently 55 of them, and nearly all are of characters released by the 2nd Anniversary of the game. If you're looking for newer characters, you're free to ignore them.
- Backup your files and don't use common names when renaming them in case anything goes wrong. I'm very inexperienced in C and batch files could be dangerous.
- The tool was tested on 19991 files (everything the game has by March 2023). One of the files will cause an error and crash, in case you run into that file, move it to another folder, and run the process again after extracting or saving your batch files (as they get replaced every run), this will be addressed in a future release. 
- I chose to remove IDs from names, and to avoid collision the extraction process will include the original file name at the start, which might make it hard to see the description if the name is long. 
- The sorting process could take a few seconds to a minute, the extraction process a minute to several, if it's taking much longer you can inform me to perhaps consider looking at its efficiency, I don't have sufficient knowledge at the moment.
- Files that share the same name and output folder will be safely ignored, it's safe to assume that's the reason some files are not being moved. 

For any questions you can contact me on discord: LostImbecile#9192.

I'll be happy to help as soon as possible, and will take any suggestions or advice regarding the code or execution process
