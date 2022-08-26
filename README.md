# BitNotify
<H1>Send Splash Screens, Popup Notifications to end users with full control.</H1>

<img width="600" alt="image" src="https://user-images.githubusercontent.com/5659686/185092477-e9e18f17-34ed-401c-9fd9-d5cd6fc69a54.png">
<b>Example:</b> PS \\Mac\Home\Downloads\bin-v10\bin> Open-SplashScreen -Title "Testing Popup" -SubTitle "This is a Subtle Subtitle" -CoverScreenArea 0.5 -BannerImage "C:\Users\Public\Documents\PersonasUsers.jpeg" -Body "C:\Users\Public\Documents\Log.txt" -Timeout 10 -ShowCloseButton $false

<img width="610" alt="image" src="https://github.com/bitsystech/BitNotify/blob/main/BitNotify%20Splash.png">
-----------------------------------------------------------------------------------------------------------------------------

<img width="600" alt="image" src="https://user-images.githubusercontent.com/5659686/185092562-2c6493f1-c325-4ac6-a3db-a94b83892f0e.png">
<b>Example:</b> PS\\Mac\Home\Downloads\bin-v10\bin> Open-Popup -Title "Helpdesk Popup" -SubTitle "This is a Restart Notification" -Body "This device has been on since Stone Age." -Image "C:\Users\Public\images\burgeretc.png" -button1 "OK" -button2 "Not Yet" -button3 "Why?" -placement "Center"
<img width="615" alt="image" src="https://github.com/bitsystech/BitNotify/blob/main/BitNotify%20Popup.png">

<h2>MANDATORY</h2>
Import-Module \\Mac\Home\Downloads\bin-v10\bin\BitNotify.dll
<br>
<i>Unless the binary is imported, the following command won’t work.</i>

To call both script, use the following:

Start-Process Powershell.exe -Argumentlist "-file \\Mac\Home\Downloads\testSplash.ps1" <br>
Start-Process Powershell.exe -Argumentlist "-file \\Mac\Home\Downloads\BNlauncher.ps1"
