## Dragon command to delete all files and folders on your dekstop

#### Step 1 create new files and folders on your Desktop

launch your Terminal and type

	$  cd ~/Desktop
   	$  mkdir  d1,d2,d3
   	$  touch file1.txt, file2.txt, file3.txt
   	
-

### Step 2 create a script to delete files and folders on your Desktop

open your favourite text editor and create the following script.

     #!/bin/bash
	 echo '' | sudo -S rm -rf /Users/yourusername/Desktop # replace yourusername

save the script and called something like removeall.sh 

make the script executable by typing into your Terminal the following command

	$ chmod u+x removeall.sh

test the cript script by typing into your Terminal 

	$ ./removeall.sh
	
directories and files on the desktop should disappear.

-

### Step 3 Create an Applescript that invokes the script

launch apple scripteditor  and type

	do shell script "bash /Users/ceo/DragonsoftwareMacautomation/removeall.sh"
	
 now re run step 1 one  to create files and folders again on your Desktop.
 
  run thw Applescript  and confirm deletion of files and folders from your desktop.
  
  export the AppleScript as  an application to  /Applications folder and  called it something like 'clear desktop.app' 

### Step 4 Use Dragon to clear desktop

 now once more create files and folders on your desktop
 
 launch Dragon and use the voice command open 'clear desktop' or whatever you have called your application 
 
 
 





	  




