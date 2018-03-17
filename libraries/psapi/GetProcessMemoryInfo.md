<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : GetProcessMemoryInfo
Group: Performance Monitoring - Library: psapi    
***  


#### Retrieves information about the memory usage of the specified process in the PROCESS_MEMORY_COUNTERS structure.
***  


## Code examples:
[Memory usage info for current VFP session (WinNT only)](../../samples/sample_172.md)  

## Declaration:
```foxpro  
BOOL GetProcessMemoryInfo(
  HANDLE Process,                          // handle to process
  PPROCESS_MEMORY_COUNTERS ppsmemCounters, // buffer
  DWORD cb                                 // size of buffer
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GetProcessMemoryInfo IN psapi;
	INTEGER  Process,;
	STRING @ ppsmemCounters,;
	INTEGER  cb  
```  
***  


## Parameters:
```txt  
Process
[in] Handle to the process.

ppsmemCounters
[out] Pointer to the PROCESS_MEMORY_COUNTERS structure that receives information about the memory usage of the process.

cb
[in] Specifies the size, in bytes, of the PROCESS_MEMORY_COUNTERS structure.
  
```  
***  


## Return value:
If the function succeeds, the return value is nonzero.  
***  


## Comments:
Windows NT/2000/XP: Included in Windows NT 4.0 and later.  
Windows 95/98/Me: Unsupported.  
  
See also WinNT Performance Monitor.  
  
See also: GetProcessIoCounters, GetProcessTimes, GetProcessVersion   
  
***  
