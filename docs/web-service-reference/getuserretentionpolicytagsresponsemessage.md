---
title: GetUserRetentionPolicyTagsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9991d6e0-8c31-4e73-8af3-da4298474b66
description: L’élément GetUserRetentionPolicyTagsResponseMessage spécifie le message de réponse pour une demande GetUserRetentionPolicyTags.
ms.openlocfilehash: 2d37a28f3babfdc5abc862338f53796ed187ec6c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515795"
---
# <a name="getuserretentionpolicytagsresponsemessage"></a>GetUserRetentionPolicyTagsResponseMessage

**L’élément GetUserRetentionPolicyTagsResponseMessage** spécifie le message de réponse pour une **demande GetUserRetentionPolicyTags.** 
  
```XML
<GetUserRetentionPolicyTagsResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RetentionPolicyTags/>
</GetUserRetentionPolicyTagsResponseMessage>
```

 **GetUserRetentionPolicyTagsResponseMessageType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [MessageXml](messagexml.md)  |  [RetentionPolicyTags](retentionpolicytags.md)
  
### <a name="parent-elements"></a>Éléments parents

[ResponseMessages](responsemessages.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |false  <br/> |
   

