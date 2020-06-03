---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: L’élément GetAttachment est l’élément racine dans une demande d’obtention d’une pièce jointe à partir de la Banque d’Exchange.
ms.openlocfilehash: d03d086ff443db87b0104a2ec83599eb9eaea6b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463978"
---
# <a name="getattachment"></a>GetAttachment

L’élément **GetAttachment** est l’élément racine dans une demande d’obtention d’une pièce jointe à partir de la Banque d’Exchange. 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 **GetAttachmentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> |Identifie les propriétés d’élément étendue supplémentaires à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) . Cet élément est facultatif.  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |Contient un tableau d’identificateurs de pièces jointes.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

L’élément [AttachmentShape](attachmentshape.md) n’est pas nécessaire pour identifier les propriétés renvoyées dans la réponse. L' [opération GetAttachment](getattachment-operation.md) renvoie les propriétés Name, ContentType, ContentId, ContentLocation et content pour les pièces jointes. Pour les pièces jointes d’éléments, les propriétés renvoyées sont le nom, ContentType, ContentId, ContentLocation, ainsi que toutes les propriétés de l’élément attaché. Cela équivaut à l’utilisation de la forme de base AllProperties dans une demande [GetItem](getitem.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetAttachment](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

