<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : SystemParametersInfo
Group: System Information - Library: user32    
***  


#### The SystemParametersInfo function retrieves or sets the value of one of the system-wide parameters. This function can also update the user profile while setting a parameter.
***  


## Code examples:
[Using the SystemParametersInfo function](../../samples/sample_283.md)  
[Displaying the associated icons and descriptions for files and folders](../../samples/sample_530.md)  
[How to find which fonts Windows uses for drawing captions, menus and message boxes](../../samples/sample_556.md)  

## Declaration:
```foxpro  
BOOL SystemParametersInfo(
  UINT uiAction,  // system parameter to retrieve or set
  UINT uiParam,   // depends on action to be taken
  PVOID pvParam,  // depends on action to be taken
  UINT fWinIni    // user profile update option
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER SystemParametersInfo IN user32;
	INTEGER   uiAction,;
	INTEGER   uiParam,;
	STRING  @ pvParam,;
	INTEGER   fWinIni  
```  
***  


## Parameters:
```txt  
uiAction
[in] Specifies the system-wide parameter to retrieve or set.

uiParam
[in] Depends on the system parameter being queried or set.

pvParam
[in/out] Depends on the system parameter being queried or set.

fWinIni
[in] If a system parameter is being set, specifies whether the user profile is to be updated.  
```  
***  


## Return value:
If the function succeeds, the return value is a nonzero value.  
***  


## Comments:
See also: GetSystemMetrics   
  
***  
