<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : WNetGetUniversalName
Group: Windows Networking - Library: mpr    
***  


#### The WNetGetUniversalName function takes a drive-based path for a network resource and returns an information structure that contains a more universal form of the name. 
***  


## Code examples:
[Retrieving a universal form for the drive-based path for a network resource](../../samples/sample_317.md)  

## Declaration:
```foxpro  
DWORD WNetGetUniversalName(
  LPCTSTR lpLocalPath,  // path for network resource
  DWORD dwInfoLevel,    // level of information
  LPVOID lpBuffer,      // name buffer
  LPDWORD lpBufferSize  // size of buffer
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER WNetGetUniversalName IN mpr;
	STRING    lpLocalPath,;
	INTEGER   dwInfoLevel,;
	STRING  @ lpBuffer,;
	INTEGER @ lpBufferSize  
```  
***  


## Parameters:
```txt  
lpLocalPath
[in] Pointer to a constant null-terminated string that is a drive-based path for a network resource.

dwInfoLevel
[in] Specifies the type of structure that the function stores in the buffer pointed to by the lpBuffer parameter.

lpBuffer
[out] Pointer to a buffer that receives the structure specified by the dwInfoLevel parameter.

lpBufferSize
[in/out] Pointer to a variable that specifies the size, in bytes, of the buffer pointed to by the lpBuffer parameter.  
```  
***  


## Return value:
If the function succeeds, the return value is NO_ERROR.  
***  
