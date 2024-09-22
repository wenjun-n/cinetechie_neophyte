With this demo, you can now create your own false colour DCTL any way you like. 

Pls note that DCTL ARE ONLY COMPATIBLE with Resolve Studio (paid version)

Please refer to the images below for the gamma comparison table. I didn't share a version with value for every 0.1 stop calculated 
as that would be too big a table to refer to, but you can refer to the Excel file named 
"Scene reflectance to log Reference Table v1.2" 
If you wish to calculate your own version, feel free to search for the various 
white papers that the respective manufacturer publishes for each gamma. 

![Gamma curve 10bit value](https://github.com/user-attachments/assets/10759fe4-83d0-4b46-99db-1744acb696fd)


![Gamma in IRE value](https://github.com/user-attachments/assets/808654cf-ddcf-4e2f-830f-fc791a8bedc8)

![Clipping point setting](https://github.com/user-attachments/assets/200cfc17-7a97-48a1-83f6-f1ccfff1df22)

The coding program I used is VS Code: https://code.visualstudio.com/download
But feel free to use your own coding program. 

You can watch this video by Kaur on the beginner's guide to DCTL development. 
https://www.youtube.com/watch?v=1BtydnVhk14

-- Log File Locations --
Win: %appdata%\Blackmagic Design\DaVinci Resolve\Support\logs\ResolveDebug.txt

Mac: /Library/Application Support/Blackmagic Design/DaVinci Resolve/logs/ResolveDebug.txt

Mac App Store: ~/Library/Containers/com.blackmagic-design.DaVinciResolveAppStore/Data/Library/Application Support/logs/ResolveDebug.txt

Linux: ~/.local/share/DaVinciResolve/logs/ResolveDebug.txt

Read more about EL zone false colour at https://www.elzonesystem.com/
