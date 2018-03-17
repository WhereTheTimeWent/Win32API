<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : URLDownloadToFile
Group: URL Monikers - Library: urlmon    
***  


#### Downloads bits from the Internet and saves them to a file.
***  


## Code examples:
[How to download a file from HTTP server using URL Monikers functions](../../samples/sample_175.md)  
[The DetectAutoProxyUrl function identifies the auto-config script location](../../samples/sample_341.md)  

## Declaration:
```foxpro  
HRESULT URLDownloadToFile(
	LPUNKNOWN pCaller,
    LPCTSTR szURL,
    LPCTSTR szFileName,
    DWORD dwReserved,
    LPBINDSTATUSCALLBACK lpfnCB
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER URLDownloadToFile IN urlmon.dll;
	INTEGER pCaller,;
	STRING  szURL,;
	STRING  szFileName,;
	INTEGER dwReserved,;
	INTEGER lpfnCB  
```  
***  


## Parameters:
```txt  
pCaller
Pointer to the controlling IUnknown interface of the calling Microsoft� ActiveX� component (if the caller is an ActiveX component). If the calling application is not an ActiveX component, this value can be set to NULL.

szURL
Pointer to a string value containing the URL to be downloaded. Cannot be set to NULL.

szFileName
Pointer to a string value containing the name of the file to create for bits that come from the download.

dwReserved
Reserved. Must be set to 0.

lpfnCB
Pointer to the caller"s IBindStatusCallback interface.  
```  
***  


## Return value:
Returns one of the following values: E_OUTOFMEMORY, S_OK  
***  
