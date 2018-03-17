<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : WNetGetConnection
Group: Windows Networking - Library: mpr    
***  


#### The WNetGetConnection function retrieves the name of the network resource associated with a local device.
***  


## Code examples:
[Retrieving the name of the network resource associated with a local device](../../samples/sample_314.md)  
[Mapping and disconnecting network drives](../../samples/sample_387.md)  

## Declaration:
```foxpro  
DWORD WNetGetConnection(
  LPCTSTR lpLocalName,  // local name
  LPTSTR lpRemoteName,  // buffer for remote name
  LPDWORD lpnLength     // buffer size
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER WNetGetConnection IN mpr;
	STRING    lpLocalName,;
	STRING  @ lpRemoteName,;
	INTEGER @ lpnLength  
```  
***  


## Parameters:
```txt  
lpLocalName
[in] Pointer to a constant null-terminated string that specifies the name of the local device to get the network name for.

lpRemoteName
[out] Pointer to a null-terminated character string buffer that receives the remote name used to make the connection.

lpnLength
[in/out] Pointer to a variable that specifies the size, in characters, of the buffer pointed to by the lpRemoteName parameter.  
```  
***  


## Return value:
If the function succeeds, the return value is NO_ERROR (0).  
***  
