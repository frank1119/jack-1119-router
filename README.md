# JackRtr1119 Readme
This repository contains (*slightly modified*) the JackRouter code from https://github.com/jackaudio/jack-router

The modifications made are done to adjust the client name by which the Jack-Router instance appears. The change is helpful to distinguish multiple instances of a particular live performance host. 

If the switch `-in=` exists on the command-line, the part after `-in=` is added to the client's executable name, separated with a dash:

Example:
```
"c:\program files\mydaw\mydaw.exe" -in=client1
```

This results in this client-name (in Jack2) `mydaw-client1`

To install the new ASIO driver:  

1. Copy the `JackRtr1119.dll` and `JackRtr1119.ini` to a folder, for example `c:\program files\JACK\jackrtr1119\win64\`
2. Open a commandbox (`cmd.exe`)
3. Register the driver, for example:  
    `regsvr32 c:\program files\JACK\jackrtr1119\win64\JackRtr1119.dll`
4. Optionally: Adjust the settings in `JackRtr1119.ini`

To uninstall the ASIO driver:  
1. Open a commandbox (`cmd.exe`)
2. Unregister the driver, for example:  
    `regsvr32 /u c:\program files\JACK\jackrtr1119\win64\JackRtr1119.dll`
3. Delete the `JackRtr1119.dll` and `JackRtr1119.ini` from the folder
