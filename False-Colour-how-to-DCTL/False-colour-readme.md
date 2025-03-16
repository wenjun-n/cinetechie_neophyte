With this demo, you can now create your own false colour DCTL any way you like. 

Pls note that DCTL ARE ONLY COMPATIBLE with Resolve Studio (paid version)
Installation of DCTL is to just copy the file to the LUT folder Davinci Resolve that is installed on your system.
Windows: C:\rogramData\Blackmagic Design\DaVinci Resolve\Support\LUT
MacOS: /Library/Application Support/Blackmagic Design/DaVinci Resolve/LUT/

DCTLs are applied by first applying "DCTL" onto your node from the effects tab on the colour page, then under the controls, you will have a dropdown box to select the DCTL you wish to use on that node. 

=== Divider ===.dctl is meant to be used as a divider when you have numerous DCTLs installed on your system, this helps searching for DCTLs faster when applying it to a node. Feel free to rename it when you move it into your LUTs folder. 

Please refer to the comments made inside the "Exposure Zone False Colour code demo.dctl" where you will find tips on how to create or make changes to your code on creating your false colour. 

Please refer to the images below for the gamma comparison table. I didn't share a version with value for every 0.1 stop calculated 
as that would be too big a table to refer to, but you can refer to the Excel file named 
"Scene reflectance to log Reference Table" 
If you wish to calculate your own version, feel free to search for the various 
white papers that the respective manufacturer publishes for each gamma. 

10bit Code Value (CV) ranges from 0-1023 for a total of 1024 steps
![Gamma curve 10bit value](https://github.com/user-attachments/assets/10759fe4-83d0-4b46-99db-1744acb696fd)

IRE value ranges from 0%-100% (if you take IRE% divide by 100 then multiply by 1023 you will get the 10bit CV.
![Gamma in IRE value](https://github.com/user-attachments/assets/808654cf-ddcf-4e2f-830f-fc791a8bedc8)

![Clipping point setting](https://github.com/user-attachments/assets/200cfc17-7a97-48a1-83f6-f1ccfff1df22)

If you wish to have a higher precision of more than four decimal places in the value used to determine your luminance range for the false colour, feel free to reference the excel sheet and reference the "scene linear to Log out data column".

Sample for setting colours for your exposure zones. Feel free to use your own set of colour and range logic for your DCTL
![Zones - float value](https://github.com/user-attachments/assets/96cc2634-17aa-4b70-99e7-9b946510f403)
<img width="1189" alt="Range logic" src="https://github.com/user-attachments/assets/bc3e1b93-1747-449e-967e-3b92a07dd1c0" />


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
