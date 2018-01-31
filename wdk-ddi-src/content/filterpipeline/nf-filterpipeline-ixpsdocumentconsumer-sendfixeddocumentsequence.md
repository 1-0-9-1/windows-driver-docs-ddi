---
UID: NF:filterpipeline.IXpsDocumentConsumer.SendFixedDocumentSequence
title: IXpsDocumentConsumer::SendFixedDocumentSequence method
author: windows-driver-content
description: The SendFixedDocumentSequence method sends a fixed document sequence to the pipeline.
old-location: print\ixpsdocumentconsumer_sendfixeddocumentsequence.htm
old-project: print
ms.assetid: e2541943-7e0c-45ca-bdfe-2d48581f62a4
ms.author: windowsdriverdev
ms.date: 1/18/2018
ms.keywords: SendFixedDocumentSequence method [Print Devices], IXpsDocumentConsumer interface, IXpsDocumentConsumer, SendFixedDocumentSequence method [Print Devices], print.ixpsdocumentconsumer_sendfixeddocumentsequence, SendFixedDocumentSequence, IXpsDocumentConsumer::SendFixedDocumentSequence, filterpipeline_cd741d5b-4069-4a67-8add-b5c2701699f6.xml, IXpsDocumentConsumer interface [Print Devices], SendFixedDocumentSequence method, filterpipeline/IXpsDocumentConsumer::SendFixedDocumentSequence
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: filterpipeline.h
req.include-header: 
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: Filterpipeline.idl
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: filterpipeline.h
req.dll: 
req.irql: 
topictype:
-	APIRef
-	kbSyntax
apitype:
-	COM
apilocation:
-	filterpipeline.h
apiname:
-	IXpsDocumentConsumer.SendFixedDocumentSequence
product: Windows
targetos: Windows
req.typenames: EXpsFontRestriction
---

# IXpsDocumentConsumer::SendFixedDocumentSequence method


## -description


The <b>SendFixedDocumentSequence</b> method sends a fixed document sequence to the pipeline.


## -syntax


````
HRESULT SendFixedDocumentSequence(
  [in] IFixedDocumentSequence *pIFixedDocumentSequence
);
````


## -parameters




#### - pIFixedDocumentSequence [in]

A pointer to an XPS fixed document sequence object.


## -returns


<code>SendFixedDocumentSequence</code> returns an <b>HRESULT</b> value.



## -remarks


Only one <a href="..\filterpipeline\nn-filterpipeline-ifixeddocumentsequence.md">IFixedDocumentSequence</a> interface can be sent. The <code>SendFixedDocumentSequence</code> method will fail if a filter submits more than one such interface for the same print job.


