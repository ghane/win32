---
Description: Adjusts the contrast.
ms.assetid: 32ae514a-eeba-4205-b6e6-70fc01b93a95
title: MFPKEY\_COLOR\_CONTRAST Property
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# MFPKEY\_COLOR\_CONTRAST Property

Adjusts the contrast.

## Constant for IPropertyBag

Available only by using [**IPropertyStore**](https://msdn.microsoft.com/windows/desktop/e995aaa1-d4c9-475f-b1fa-b9123cd5b653).

## Data Type

VT\_I4

## Default Value

0

## Applies To

-   [Color Control Transform DSP](colorcontroltransform.md)

## Remarks

Contrast adjustment is performed by multiplying the YCbCr values by a scaling factor.

This property has a range of -127 to 127. Zero indicates no change in contrast.

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                             |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                    |
| Header<br/>                   | <dl> <dt>Wmcodecdsp.h</dt> </dl> |



## See also

<dl> <dt>

[Media Foundation Properties](media-foundation-properties.md)
</dt> </dl>

 

 



