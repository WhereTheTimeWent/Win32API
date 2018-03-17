<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : CeCreateDatabase
Group: Remote Application Programming (RAPI) - Library: rapi    
***  


#### This function creates a new database.
***  


## Code examples:
[Pocket PC: custom RAPI class for operating with the Object Store Databases](../../samples/sample_445.md)  

## Declaration:
```foxpro  
CEOID CeCreateDatabase(
  LPWSTR lpszName,
  DWORD dwDbaseType,
  WORD wNumSortOrder,
  SORTORDERSPEC* rgSortSpecs
);  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER CeCreateDatabase IN rapi;
	STRING  lpszName,;
	INTEGER dwDbaseType,;
	SHORT   wNumSortOrder,;
	INTEGER rgSortSpecs
  
```  
***  


## Parameters:
```txt  
lpszName
[in] Long pointer to a null-terminated string that specifies the name for the new database.

dwDbaseType
[in] Specifies the type identifier for the database.

wNumSortOrder
[in] Number of sort orders active in the database, with four being the maximum number.

rgSortSpecs
[in] Pointer to an array of actual sort order descriptions.  
```  
***  


## Return value:
The object identifier of the newly created database � not a handle to an open database � indicates success.  
***  


## Comments:
The name can have up to 32 characters, including the terminating null character.  
  
See also CeOpenDatabase, CeDeleteDatabase, CeWriteRecordProps and CeDeleteRecord functions.  
  
***  
