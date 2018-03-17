<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : IsValidURL
Group: URL Monikers - Library: urlmon    
***  


#### Determines if a specified string is a valid URL.
***  


## Code examples:
[Validating URLs using moniker functions](../../samples/sample_194.md)  

## Declaration:
```foxpro  
HRESULT IsValidURL(
	LPBC pBC,
	LPCWSTR szURL,
	DWORD dwReserved
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER IsValidURL IN urlmon;
	INTEGER pBC,;
	STRING  szURL,;
	INTEGER dwReserved  
```  
***  


## Parameters:
```txt  
pBC
[in] Pointer to the IBindCtx interface. This parameter is currently ignored. It should be set to NULL.

szURL
[in] Pointer to a string value that contains the full URL to be checked.

dwReserved
[in] Reserved. Must be set to 0.  
```  
***  


## Return value:
Returns one of the following values:
S_OK = 0
S_FALSE = 1
E_INVALIDARG = 0x80070057  
***  
