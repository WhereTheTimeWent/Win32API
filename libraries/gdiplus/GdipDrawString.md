<link rel="stylesheet" type="text/css" href="../../css/win32api.css">  
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

## Functionname : GdipDrawString
Group: GDI+ Text - Library: gdiplus    
***  


#### Draws a string based on a font, a layout rectangle, and a format
***  


## Code examples:
[Custom GDI+ class](../../samples/sample_450.md)  

## Declaration:
```foxpro  
GpStatus WINGDIPAPI GdipDrawString(
	GpGraphics *graphics,
	GDIPCONST WCHAR *string,
	INT length,
	GDIPCONST GpFont *font,
	GDIPCONST RectF *layoutRect,
	GDIPCONST GpStringFormat *stringFormat,
	GDIPCONST GpBrush *brush
)
  
```  
***  


## FoxPro declaration:
```foxpro  
DECLARE INTEGER GdipDrawString IN gdiplus;
	INTEGER   graphics,;
	STRING    widechar,;
	INTEGER   length,;
	INTEGER   fnt,;
	STRING  @ rectf,;
	INTEGER   stringFormat,;
	INTEGER   brush  
```  
***  


## Parameters:
```txt  
graphics
[in] Pointer to a Graphics object.

string
[in] Pointer to a wide-character string to be drawn.

length
[in] Integer that specifies the number of characters in the string array. The length parameter can be set to �1 if the string is null terminated.

font
[in] Pointer to a Font object that specifies the font attributes (the family name, the size, and the style of the font) to use.

layoutRect
[in] Reference to a rectangle (of floats) that bounds the string.

stringFormat
[in] Pointer to a StringFormat object that specifies text layout information and display manipulations to be applied to the string.

brush
[in] Pointer to a Brush object that is used to fill the string.
  
```  
***  


## Return value:
If the method succeeds, it returns Ok (0), which is an element of the Status enumeration.  
***  


## Comments:
Note that the <Em>layoutRect</Em> structure contains four 32-bit float numbers, not four 32-bit INT numbers.  
  
Presented in this reference <a href="?example=450">GDI+ class</a> uses <Em>float2int</Em> conversion routine to populate this structure:<code><font color=#0000a0>  
FUNCTION RECTF(nLeft, nTop, nRight, nBottom)  
RETURN num2dword(Int2Float(nLeft)) + num2dword(Int2Float(nTop)) +;  
	num2dword(Int2Float(nRight)) + num2dword(Int2Float(nBottom))  
</font></code>  
  
***  
