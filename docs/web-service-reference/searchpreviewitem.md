---
title: SearchPreviewItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 59b0b2db-a0ae-4162-a2cb-5f37f42fe872
description: L’élément SearchPreviewItem spécifie l’aperçu d’élément pour une recherche de découverte.
ms.openlocfilehash: 7ecc034de3386ed35f0071403c013e91b79d13c5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534300"
---
# <a name="searchpreviewitem"></a>SearchPreviewItem

**L’élément SearchPreviewItem** spécifie l’aperçu d’élément pour une recherche de découverte. 
  
```XML
<SearchPreviewItem>
   <Id/>
   <Mailbox/>
   <ParentId/>
   <ItemClass/>
   <UniqueHash/>
   <SortValue/>
   <OwaLink/>
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <CreatedTime/>
   <ReceivedTime/>
   <SentTime/>
   <Subject/>
   <Size/>
   <Preview/>
   <Importance/>
   <Read/>
   <HasAttachment/>
   <ExtendedProperties/>
</SearchPreviewItem>
```

 **SearchPreviewItemType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[ID (ItemIdType)](id-itemidtype.md)  |  [Mailbox (PreviewItemMailboxType)](mailbox-previewitemmailboxtype.md)  |  [ParentId](parentid.md)  |  [ItemClass](itemclass.md)  |  [UniqueHash](uniquehash.md)  |  [SortValue](sortvalue.md)  |  [OwaLink](owalink.md)  |  [Expéditeur (chaîne)](sender-string.md)  |  [ToRecipients (ArrayOfSmtpAddressType)](torecipients-arrayofsmtpaddresstype.md)  |  [CcRecipients](ccrecipients.md)  |  [BccRecipients](bccrecipients.md)  |  [CreatedTime](createdtime.md)  |  [ReceivedTime](receivedtime.md)  |  [SentTime](senttime.md)  |  [Objet](subject.md)  |  [Taille (longue)](size-long.md)  |  [Aperçu](preview-ex15websvcsotherref.md)  |  [Importance](importance.md)  |  [Lecture](read.md)  |  [HasAttachment](hasattachment.md)  |  [ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)](extendedproperties-nonemptyarrayofextendedpropertytype.md)
  
### <a name="parent-elements"></a>Éléments parents

[Items (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

