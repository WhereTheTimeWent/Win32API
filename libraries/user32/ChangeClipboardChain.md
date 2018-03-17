<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : ChangeClipboardChain
Group: Clipboard - Library: user32    
***  


#### Removes a specified window from the chain of clipboard viewers.
***  


## Code examples:
[How to disable the Windows Clipboard (VFP9)](../../samples/sample_488.md)  

## Declaration:
```foxpro  
BOOL ChangeClipboardChain(
	HWND hWndRemove,
	HWND hWndNewNext
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER ChangeClipboardChain IN user32;
	INTEGER hWndRemove,;
	INTEGER hWndNewNext
  
```  
***  


## Parameters:
```txt  
hWndRemove
[in] Handle to the window to be removed from the chain. The handle must have been passed to the SetClipboardViewer function.

hWndNewNext
[in] Handle to the window that follows the hWndRemove window in the clipboard viewer chain.  
```  
***  


## Return value:
... is indecisive. 

It indicates the result of passing the WM_CHANGECBCHAIN message to the windows in the clipboard viewer chain. Because a window in the chain typically returns FALSE when it processes WM_CHANGECBCHAIN, the return value from ChangeClipboardChain is typically FALSE.  
***  


## Comments:
The window identified by hWndNewNext replaces the hWndRemove window in the chain. The SetClipboardViewer function sends a WM_CHANGECBCHAIN message to the first window in the clipboard viewer chain.   
  
See also: SetClipboardViewer, AddClipboardFormatListener, RemoveClipboardFormatListener   
  
***  
