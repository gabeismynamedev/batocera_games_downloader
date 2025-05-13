# Batocera PyGame Downloader
This app does not endorse any kind of piracy.

This is a simple tool to help download games to your console.

This is tested with Knulli RG35xxSP. I dont have time or desire to test in other console.

To install in your console, create a downloader foler inside the pygame roms folder and add those two files, modify the download.json with your links. 
Add your urls, I am giving examples using internet archive. ( I may delete those examples to avoid people to use to piracy).

On emulationstation rescan all your games, go to the pygame library and the run the app.

Only download games you own a copy.


JSON STRUCTURE

````
 {
    "name": NAME OF THE SYSTEM,
    "list_url": URL TO GET A JSON WITH ALL FILES,
    "list_json_file_location": THE JSON PROPERTY NAME WHERE THE ARRAY OF FILES IS,
    "list_item_id": THE IDENTIFIER PROPERTY OF EACH GAME,
    "download_url": THE DOWNLOAD URL, ITS GOING TO BE CONCATENATED WITH THE IDENTIFIER. EG.: https:test.com/{ID},
    "commands": AN ARRAY OF BASH COMMANDS IN CASE YOU NEED TO UNZIP OR ANYTHING (NOT WORKING),
    "file_format": [".iso"] AN ARRAY OF THE FILE FORMATS THAT WILL BE LISTED, DOWNLOADED AND MOVED TO THE FOLDER,
    "roms_folder": THE NAME OF THE FOLDER INSIDE ROMS FOLDER THAT GAMES SHOULD BE MOVED AFTER DOWNLOAD
  },
````

Tested only with links of Internet Archive.


If you want to contribute feel free to submit a PR.
