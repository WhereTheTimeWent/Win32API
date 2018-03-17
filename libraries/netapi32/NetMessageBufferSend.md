<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : NetMessageBufferSend
Group: Network Management - Library: netapi32    
***  


#### Sends a buffer of information to a registered message alias.

***  


## Code examples:
[Using the NetMessageBufferSend to send messages on the network](../../samples/sample_494.md)  

## Declaration:
```foxpro  
NET_API_STATUS NetMessageBufferSend(
	LPCWSTR servername,
	LPCWSTR msgname,
	LPCWSTR fromname,
	LPBYTE buf,
	DWORD buflen
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER NetMessageBufferSend IN netapi32;
	STRING   servername,;
	STRING   msgname,;
	STRING   fromname,;
	STRING @ buf,;
	INTEGER  buflen  
```  
***  


## Parameters:
```txt  
servername
[in] Pointer to a constant string that specifies the DNS or NetBIOS name of the remote server on which the function is to execute. If this parameter is NULL, the local computer is used.

msgname
[in] Pointer to a constant string that specifies the message alias to which the message buffer should be sent.

fromname
[in] Pointer to a constant string specifying who the message is from. If this parameter is NULL, the message is sent from the local computer name.

buf
[in] Pointer to a buffer that contains the message text.

buflen
[in] Specifies a value that contains the length, in bytes, of the message text pointed to by the buf parameter.  
```  
***  


## Return value:
If the function succeeds, the return value is NERR_Success (0).  
***  


## Comments:
Admin, Accounts, Print, or Server Operator group membership is required to successfully execute NetMessageBufferSend on a remote server.  
  
Can be used as NET SEND replacement.  
Note that this is Unicode function.  
Not supported on Win9* systems.  
  
See also: NetMessageNameEnum, NetMessageNameAdd, NetMessageNameDel.  
  
***  
