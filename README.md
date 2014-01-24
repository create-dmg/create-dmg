	----------------------------------------------------------
	YourSway create dmg
	----------------------------------------------------------
	Creates a fancy DMG file, complete with custom image background, 
	specified icon positions and set to open in the Icon View. 
	----------------------------------------------------------
	1. Create a directory (source_folder), then put all the files 
	   you'll want in your final .dmg in this directory. Typically this 
	   includes your .app, a background.png, and a documentation file.
	2. Run the create-dmg script from your terminal, pass in your custom 
	   options, and your dmg will be generated!

	----------------------------------------------------------
	Basic Example: 
	----------------------------------------------------------
	./create-dmg \
		--volname "YourAppName" \
		--volicon ./yourIcon.icns \
		--background ./yourBackground.png \
		--window-size 500 300 \
		--icon-size 96 \
		--app-drop-link 398 181 \
		--icon "YourApp" 109 181 \
		YourAppName.dmg ./source_folder/

	----------------------------------------------------------
	Options:
	----------------------------------------------------------
	  --volname name
		  set volume name (displayed in the Finder sidebar & window title)
	  --volicon yourIcon.icns
		  set volume icon
	  --background yourImage.png
		  set folder background image (supports png, gif or jpg)
	  --window-pos x y
		  set position the folder window
	  --window-size width height
		  set size of the folder window
	  --icon-size icon_size
		  set window icons size (up to 128)
	  --icon file_name x y
		  set position of the file's icon
	  --hide-extension file_name
		  hide the extension of file
	  --custom-icon file_name custom_icon_or_sample_file x y
		  set position and custom icon
	  --app-drop-link x y
		  make a drop link to Applications, at location x,y
	  --eula eula_file
		  attach a license file to the dmg
	  --no-internet-enable
		  disable automatic mount&copy
	
	----------------------------------------------------------
	Requirements:
	----------------------------------------------------------
	OSX
	
	----------------------------------------------------------
	License:
	----------------------------------------------------------
	This tool is licensed under GNU General Public License, because it 
	incorporates portions of GPL-licensed code from Adium repository. 
	You can modify this program to suite your needs, but you have to 
	provide the source code of any modifications upon request.
