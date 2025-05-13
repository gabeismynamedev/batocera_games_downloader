# Batocera PyGame Downloader
This app is not endorse any kind of piracy.

This is a simple tool to help download games to your console.

This is tested with Knulli RG35xxSP. I dont have time or desire to test in other console.

To install in your console, create a downloader foler inside the pygame roms folder and add those two files. 
Add your urls, I am giving examples using internet archive. ( I may delete those examples to avoid people to use to piracy).

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

