---
Description: 'Specifies the maximum reference frames supported by the encoder.'
ms.assetid: '023FD791-BD43-41F6-95D0-8BE800F51579'
title: 'CODECAPI\_AVEncVideoMaxNumRefFrame property'
---

# CODECAPI\_AVEncVideoMaxNumRefFrame property

Specifies the maximum reference frames supported by the encoder.

## Data type

**ULONG** (VT\_UI4)

## Property GUID

**CODECAPI\_AVEncVideoMaxNumRefFrame**

## Remarks

For H.264, this maps to the Sequence Parameter Set variable **max\_num\_ref\_frames** as defined in H.264 specification.

**H.264/AVC encoders:**

Encoders may use fewer reference frames in order to obey the level specified in the bitstream.

Encoders shall support [**GetValue**](imfmediaevent-getvalue.md), [**SetValue**](https://msdn.microsoft.com/library/windows/desktop/dd311966), and [**GetParameterRangee**](https://msdn.microsoft.com/library/windows/desktop/dd311956).

This is a static property meaning that it can only be set before the encoding session starts.

Recommended default value is 2.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�8.1 \[desktop apps \| UWP apps\]<br/>                                   |
| Minimum supported server<br/> | Windows Server�2012�R2 \[desktop apps \| UWP apps\]<br/>                        |
| Header<br/>                   | <dl> <dt>Codecapi.h</dt> </dl> |



## See also

<dl> <dt>

[Media Foundation Properties](media-foundation-properties.md)
</dt> </dl>

�

�



