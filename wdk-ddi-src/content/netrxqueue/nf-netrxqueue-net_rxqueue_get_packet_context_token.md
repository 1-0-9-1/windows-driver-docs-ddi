---
UID: NF:netrxqueue.NET_RXQUEUE_GET_PACKET_CONTEXT_TOKEN
title: NET_RXQUEUE_GET_PACKET_CONTEXT_TOKEN macro
author: windows-driver-content
description: The NET_RXQUEUE_GET_PACKET_CONTEXT_TOKEN macro retrieves the token identifier for a packet context, for receive queues that use more than one packet context.
ms.assetid: d6aa295b-afb0-401b-bf4f-7725c528a68d
ms.author: windowsdriverdev
ms.date: 02/09/2018
ms.topic: macro
ms.keywords: NET_RXQUEUE_GET_PACKET_CONTEXT_TOKEN
req.header: netrxqueue.h
req.include-header: netadaptercx.h
req.target-type: Universal
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver: 1.23
req.umdf-ver:
req.lib:
req.dll:
req.irql: 
req.ddi-compliance:
req.unicode-ansi:
req.idl:
req.max-support:
req.namespace:
req.assembly:
req.type-library: 
req.alt-api:
req.alt-loc:
topictype: 
-	apiref
apitype: 
-	HeaderDef
apilocation: 
-	netrxqueue.h
apiname: 
-	NET_RXQUEUE_GET_PACKET_CONTEXT_TOKEN
product: Windows
targetos: Windows
req.product: Windows 10 or later.
---

# NET_RXQUEUE_GET_PACKET_CONTEXT_TOKEN macro


## -description

> [!WARNING]
> Some information in this topic relates to prereleased product, which may be substantially modified before it's commercially released. Microsoft makes no warranties, express or implied, with respect to the information provided here.
>
> NetAdapterCx is preview only in Windows 10, version 1809.

The **NET_RXQUEUE_GET_PACKET_CONTEXT_TOKEN** macro retrieves the token identifier for a packet context, for receive queues that use more than one packet context.

## -parameters

### -param _rxqueue
A handle to the NETRXQUEUE object.

### -param _contexttype
The structure type name of a driver-defined structure that describes the contents of the packet's context space.

## -remarks
Queues with more than one packet per context require a **NET_PACKET_CONTEXT_TOKEN** to identify and retrieve each context. Call **NET_RXQUEUE_GET_PACKET_CONTEXT_TOKEN** to retrieve the token for a context type if your receive queue uses more than one context per packet.

For an example of how to use this macro to retrieve a packet context token, see [NET_PACKET_DECLARE_CONTEXT_TYPE_WITH_NAME](../netadapterpacket/nf-netadapterpacket-net_packet_declare_context_type_with_name.md).



## -see-also