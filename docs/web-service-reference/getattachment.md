---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: L’élément GetAttachment est l’élément racine d’une demande d’obtenir une pièce jointe à partir Exchange store.
ms.openlocfilehash: 057b42e78845f583cf1e52804e0108f335ef951c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546370"
---
# <a name="getattachment"></a>GetAttachment

**L’élément GetAttachment** est l’élément racine d’une demande d’obtenir une pièce jointe à partir Exchange store. 
  
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
|[AttachmentShape](attachmentshape.md) <br/> |Identifie d’autres propriétés d’élément étendu à renvoyer dans une réponse à [une demande GetAttachment.](getattachment.md) Cet élément est facultatif.  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |Contient un tableau d’identificateurs de pièces jointes.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

[L’élément AttachmentShape](attachmentshape.md) n’est pas nécessaire pour identifier les propriétés renvoyées dans la réponse. [L’opération GetAttachment](getattachment-operation.md) renvoie les propriétés Name, ContentType, ContentId, ContentLocation et ContentLocation pour les pièces jointes de fichier. Pour les pièces jointes d’élément, les propriétés renvoyées sont Name, ContentType, ContentId, ContentLocation et toutes les propriétés de l’élément joint. Cela équivaut à utiliser la forme de base AllProperties dans une [requête GetItem.](getitem.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetAttachment](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

