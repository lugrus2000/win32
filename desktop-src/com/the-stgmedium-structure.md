---
title: The STGMEDIUM Structure
description: The STGMEDIUM Structure
ms.assetid: 'ff1e1128-d228-45a6-a19d-2875b6c4e003'
---

# The STGMEDIUM Structure

Just as the [**FORMATETC**](formatetc.md) structure is an enhancement of the Windows clipboard format identifier, so the [**STGMEDIUM**](stgmedium.md) structure is an improvement of the global memory handle used to transfer the data. The **STGMEDIUM** structure includes a member, **tymed**, which indicates the medium to be used, and a union comprising pointers and a handle for getting whichever medium is specified in **tymed**.

The [**STGMEDIUM**](stgmedium.md) structure enables both data sources and consumers to choose the most efficient exchange medium on a per-rendering basis. If the data is so large that it should be kept on disk, the data source can indicate a disk-based medium in its preferred format, only using global memory as a backup if that's the only medium the consumer understands. Being able to use the best medium for exchanges as the default improves overall performance of data exchange between applications. For example, if some of the data to be transferred is already on disk, the source application can move or copy it to a new destination, either in the same application or in some other, without having first to load the data into global memory. At the receiving end, the consumer of the data does not have to write it back to disk.

## Related topics

<dl> <dt>

[Data Formats and Transfer Media](data-formats-and-transfer-media.md)
</dt> </dl>

 

 



