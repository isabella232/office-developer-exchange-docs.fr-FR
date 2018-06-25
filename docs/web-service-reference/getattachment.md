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
description: L’élément GetAttachment est l’élément racine dans une demande pour obtenir une pièce jointe à partir de la banque d’informations Exchange.
ms.openlocfilehash: fb639c86a0654e8f9e9601310f7c2f5b0fc7d729
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756524"
---
# <a name="getattachment"></a>GetAttachment

L’élément **GetAttachment** est l’élément racine dans une demande pour obtenir une pièce jointe à partir de la banque d’informations Exchange. 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 **GetAttachmentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> |Identifie les propriétés totale de l’article à renvoyer dans une réponse à une demande [GetAttachment](getattachment.md) . Cet élément est facultatif.  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |Contient un tableau d’identificateurs de pièce jointe.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

L’élément [AttachmentShape](attachmentshape.md) n’est pas nécessaire pour identifier les propriétés renvoyées dans la réponse. L' [opération GetAttachment](getattachment-operation.md) renvoie le nom, ContentType, ContentId, ContentLocation et les propriétés du contenu des pièces jointes. Les pièces jointes d’élément, les propriétés retournées sont le nom, ContentType, ContentId, ContentLocation et toutes les attaché propriétés de l’élément. Cela équivaut à l’utilisation de la forme de base AllProperties dans une demande de [GetItem](getitem.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetAttachment](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

