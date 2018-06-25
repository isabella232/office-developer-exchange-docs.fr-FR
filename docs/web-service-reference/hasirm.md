---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: L’élément HasIrm indique si au moins un message dans la conversation et le dossier actif est un message protégé IRM.
ms.openlocfilehash: c129370d7920da7cf1f9f32eed2f075e6c21cf8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827803"
---
# <a name="hasirm"></a>HasIrm

L’élément **HasIrm** indique si au moins un message dans la conversation et le dossier actif est un message protégé IRM. 
  
```XML
<HasIrm> true | false </HasIrm>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Conversation (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **HasIrm** est **la valeur true** si au moins un message dans la conversation et le dossier actif a IRM. Dans le cas contraire, la valeur est **false**.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Conversation (ConversationType)](conversation-conversationtype.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

