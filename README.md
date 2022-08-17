# BitNotify
Send Splash Screens, Popup Notifications to end users with full control.
Open-SplashScreen	-Title	Enter the title
	-Subtitle	Enter any subtitle
	-BannerImage	Path to png file
	-CoverScreenArea	D
	-Body	Or BeginReading
	-BeginReading	Give path of file in which your other script will keep writing whatever it’s doing, that you want to show to the user. 
	-Timeout	In seconds
	-ShowCloseButton	$true or $false (for False, you can just skip -ShowCloseButton
	-ExitBinaryANDRestart	This can’t be clubbed with the commands above. Needs to be executed separately. It’s recommended not to use, rather do device restart using your main script. 
	Mandatory	" Import-Module \\Mac\Home\Downloads\bin-v10\bin\BitNotify.dll 

Unless the binary is imported, the following command won’t work.     "
	Example
  PS \\Mac\Home\Downloads\bin-v10\bin> Open-SplashScreen -Title "Testing Popup" -SubTitle "This is a Subtle Subtitle" -CoverScreenArea 0.5 -BannerImage "C:\Users\Public\Documents\PersonasUsers.jpeg" -Body "C:\Users\Public\Documents\Log.txt" -Timeout 10 -ShowCloseButton $false<img width="562" alt="image" src="https://user-images.githubusercontent.com/5659686/185092477-e9e18f17-34ed-401c-9fd9-d5cd6fc69a54.png">



		
Open-Popup	-Title	Enter the title
	-Subtitle	Enter any subtitle
	-Body	Detailed info, it can show scroll button if the text is too long.
	-Image	This is the icon we want to show
	-button1, -button2, -button3	Add text on button
	-placement	Center, TopRight, BottomRight
	Mandatory	" Import-Module \\Mac\Home\Downloads\bin-v10\bin\BitNotify.dll 

Unless the binary is imported, the following command won’t work.     "
	Example 	
  PS\\Mac\Home\Downloads\bin-v10\bin> Open-Popup -Title "Helpdesk Popup" -SubTitle "This is a Restart Notification" -Body "This device has been on since Stone Age." -Image "C:\Users\Public\images\burgeretc.png" -button1 "OK" -button2 "Not Yet" -button3 "Why?" -placement "TopRight"<img width="582" alt="image" src="https://user-images.githubusercontent.com/5659686/185092562-2c6493f1-c325-4ac6-a3db-a94b83892f0e.png">
