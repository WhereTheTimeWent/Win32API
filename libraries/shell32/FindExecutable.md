<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : FindExecutable
Group: Shell Functions - Library: shell32    
***  


#### Retrieves the name of and handle to the executable (.exe) file associated with the specified file name.
***  


## Code examples:
[Accessing the list of Windows Recent Documents](../../samples/sample_094.md)  
[How to find the application associated with a file name](../../samples/sample_138.md)  
[How to make application automatically close all documents it opened](../../samples/sample_491.md)  

## Declaration:
```foxpro  
HINSTANCE FindExecutable(
    LPCTSTR lpFile,
    LPCTSTR lpDirectory,
    LPTSTR lpResult
);
  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER FindExecutable IN shell32;
	STRING lpFile,;
	STRING lpDirectory,;
	STRING @lpResult  
```  
***  


## Parameters:
```txt  
lpFile
Address of a null-terminated string specifying a file name. This should be a document.

lpDirectory
Address of a null-terminated string specifying the default directory.

lpResult
Address of a buffer to receive the file name when the function returns.  
```  
***  


## Return value:
Returns a value greater than 32 if successful, or a value less than or equal to 32 otherwise.  
***  


## Comments:
See also: ShellExecute, AssocQueryString   
  
***  
