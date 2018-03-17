<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : GetMailslotInfo
Group: Mailslot - Library: kernel32    
***  


#### The GetMailslotInfo function retrieves information about the specified mailslot. 
***  


## Code examples:
[Creating a mailslot](../../samples/sample_267.md)  
[Peer-to-peer LAN messenger built with Mailslot API functions](../../samples/sample_410.md)  

## Declaration:
```foxpro  
BOOL GetMailslotInfo(
  HANDLE hMailslot,          // mailslot handle
  LPDWORD lpMaxMessageSize,  // maximum message size
  LPDWORD lpNextSize,        // size of next message
  LPDWORD lpMessageCount,    // number of messages
  LPDWORD lpReadTimeout      // read time-out interval
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GetMailslotInfo IN kernel32;
	INTEGER   hMailslot,;
	INTEGER @ lpMaxMessageSize,;
	INTEGER @ lpNextSize,;
	INTEGER @ lpMessageCount,;
	INTEGER @ lpReadTimeout  
```  
***  


## Parameters:
```txt  
hMailslot
[in] Handle to a mailslot. The CreateMailslot function must create this handle.

lpMaxMessageSize
[in] Pointer to a buffer specifying the maximum message size, in bytes, allowed for this mailslot, when the function returns.

lpNextSize
[in] Pointer to a buffer specifying the size, in bytes, of the next message, when the function returns.

lpMessageCount
[in] Pointer to a buffer specifying the total number of messages waiting to be read, when the function returns.

lpReadTimeout
[in] Pointer to a buffer specifying the amount of time, in milliseconds, a read operation can wait for a message to be written to the mailslot before a time-out occurs.  
```  
***  


## Return value:
If the function succeeds, the return value is nonzero.  
***  
