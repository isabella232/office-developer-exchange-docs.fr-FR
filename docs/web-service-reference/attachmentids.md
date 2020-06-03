---
title: AttachmentIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentIds
api_type:
- schema
ms.assetid: 46ce3ad7-4b20-43ae-8c63-39f1e3c2666b
description: L’élément AttachmentIds contient un tableau d’identificateurs de pièces jointes.
ms.openlocfilehash: cff1cb5658690fd6dd2c6a7812e1f600a4c80e29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464251"
---
# <a name="attachmentids"></a>AttachmentIds

L’élément **AttachmentIds** contient un tableau d’identificateurs de pièces jointes. 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 **NonEmptyArrayOfRequestAttachmentIdsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentId (GetAttachment et DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) <br/> |Élément qui identifie une pièce jointe unique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DeleteAttachment](deleteattachment.md) <br/> |Élément qui définit une demande de suppression d’une pièce jointe de la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/DeleteAttachment` <br/> |
|[GetAttachment](getattachment.md) <br/> |Élément qui définit une demande d’obtention d’une pièce jointe à partir de la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération DeleteAttachment](deleteattachment-operation.md)
- [Opération GetAttachment](getattachment-operation.md)

