

This repository contains (*slightly midified*) the JackRouter code from https://github.com/jackaudio/jack-router

The modifications made are done to adjust the client name by which the Jack-Router instance appears. The change is helpful to distinguish multiple instances of a particular live performance host. 

If the switch '-in=' exists on the command-line, the part after '-in=' is added to the client's executable name:

Example
```
"c:\program files\mydaw\mydaw.exe" -in=client1
```

This results in this client-name (in Jack2):

```
mydaw-client1
```
