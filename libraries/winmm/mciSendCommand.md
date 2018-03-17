<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : mciSendCommand
Group: Windows Multimedia - Library: winmm    
***  


#### Sends a command message to the specified MCI device.
***  


## Declaration:
```foxpro  
MCIERROR mciSendCommand(
	MCIDEVICEID IDDevice,
	UINT uMsg,
	DWORD fdwCommand,
	DWORD_PTR dwParam
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER mciSendCommand IN winmm;
	INTEGER IDDevice,;
	LONG uMsg,;
	LONG fdwCommand,;
	LONG dwParam
  
```  
***  


## Parameters:
```txt  
IDDevice
Device identifier of the MCI device that is to receive the command message. This parameter is not used with the MCI_OPEN command message.

uMsg
Command message, a multimedia command.

fdwCommand
Flags for the command message.

dwParam
Pointer to a structure that contains parameters for the command message.  
```  
***  


## Return value:
Returns zero if successful or an error otherwise.  The low-order word of the returned DWORD value contains the error return value.

To retrieve a text description of return values, pass the return value to the mciGetErrorString function.  
***  


## Comments:
<a href="http://msdn.microsoft.com/en-us/library/dd743571(VS.85).aspx">List of Multimedia Commands</a> on MSDN.  
  
See also: mciSendString, mciGetDeviceID   
  
***  
