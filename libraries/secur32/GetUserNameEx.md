<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : GetUserNameEx
Group: System Information - Library: secur32    
***  


#### Retrieves the name of the user or other security principal associated with the calling thread. You can specify the format of the returned name.
***  


## Declaration:
```foxpro  
BOOLEAN WINAPI GetUserNameEx(
  __in     EXTENDED_NAME_FORMAT NameFormat,
  __out    LPTSTR lpNameBuffer,
  __inout  PULONG lpnSize
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GetUserNameEx IN secur32;
	INTEGER NameFormat,;
	STRING @lpNameBuffer,;
	LONG @lpnSize  
```  
***  


## Parameters:
```txt  
NameFormat [in]
The format of the name. This parameter is a value from the EXTENDED_NAME_FORMAT enumeration type.

lpNameBuffer [out]
A pointer to a buffer that receives the name in the specified format.

lpnSize [in, out]
On input, this variable specifies the size of the lpNameBuffer buffer, in TCHARs.  
```  
***  


## Return value:
If the function succeeds, the return value is a nonzero value.  
***  


## Comments:
If the thread is impersonating a client, GetUserNameEx returns the name of the client.  
  
***  
