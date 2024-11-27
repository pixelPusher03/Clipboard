# SMPaste 
 A tool to perform clipboard poisoning or paste jacking attack. There are many tools for performing this type of attack but I found most of them are dead and none of them provides user to use their own html files, so I came up with this. 

  
 ## What's Clipboard Poisoning or PasteJacking ? 
 Browsers now allow developers to automatically add content to a user's clipboard and the attacker exploits this feature. It is a type of attack where the malicious websites take control of your device's clipboard and replace it's content to something harmful without your knowledge.</br>This method can be used to entice users into running seemingly innocent commands. The malicious code will override the innocent code, and the attacker can gain remote code execution on the user's host if the user pastes the contents into the terminal. 
  
 ## Screenshot 
 <img src="![Screenshot_20231023-205430~2](https://github.com/thedeveloper03/smpaste/assets/123274423/85b9f3b0-f171-495d-b0d0-e383e92b9c44)
" width="100%"></img> 
  
 ## Usage 
 + Enter command to inject :</br> 
 Be careful with this, it is the command which will be get excuted when the target copies something from our website and pastes it into the terminal. Know your target first before entering the command, if its windows type the windows commands and same for the Linux. 
 + Enable anonymous mode (y/n) :</br> 
 The anonymous mode clears the terminal after executing the injected command and cleares the history as well, so no logs are being created. Please note that use anonymous mode if your target is Linux for Windows append "***;clear***" at the end of the command. 
 + HTML file to infect (path) :</br> 
 Enter the path to the HTML file, where it is stored on your device. Make sure your file contains ***\<body>*** tag else the script will show an error. 
  
  
 ## Installing and requirements 
 - Linux or Unix-based system 
  
 ### Installing 
 ``` 
 ~ ❯❯❯ git clone https://github.com/thedeveloper03/smpaste.git 
  
 ~ ❯❯❯ cd smpaste
  
 ~ ❯❯❯ chmod +x smpaste.sh 
  
 ~ ❯❯❯ ./smpaste.sh 
 ``` 
   
 ## Disclaimer 
  
 SMPaste is created to help in penetration testing and it's not responsible for any misuse or illegal purposes. 