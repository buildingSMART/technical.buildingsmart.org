String Encoding & Decoding
==========================

The IFC exchange format “STEP physical file” uses characters represented by decimal value 32 to 126 from the code table in ISO 8859-1. Any other character, like some Western characters, like the German “Umlaut”, Greek or Cyrillic letters, or Asian characters, has to be encoded before being exchanged as part of a string value. Up until IFC4.x this encoding is used in IFC. In the future, IFC will adopt the UTF8 encoding. 

> The rules for decoding and encoding are defined in ISO10303-21: “_Industrial automation systems and integration — Product data representation and exchange — Part 21: Implementation methods: Clear text encoding of the exchange structure_“. A short summary and guideline is included in the IFC Implementation Guide.

**_Example:_** The following encodings define the character “Upper A umlaut” Ä – the hexadecimal character code is xC4 (decimal 196)

| Characters | Description |
| --- | --- |
| ‘\\S\\D’ | character code of D = x44 (decimal 68) added to x80 (128) is  x44 + x80 (68+128) = xC4 (196); since Ä is defined in ISO 8859-1 it is the default code page and no P encoding is required. |
| ‘\\PA\\\\S\\D’ | same as above, but the PA directive at the begin of the string explicitly defines that the value of xC4 (196) is taken from ISO 8859-1 |
| ‘\\X\\C4’ | character code xC4 as 8-bit character code found in ISO 10646 (first 255 characters – also referred to as “row 0”) |
| ‘\\X2\\00C4\\X0\\’ | character code xC4 as 16-bit character x00C4 in ISO 10646 (Unicode) |
