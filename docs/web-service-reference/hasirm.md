---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: L’élément HasIrm spécifie si au moins un message dans la conversation et le dossier actuel est un message protégé par IRM.
ms.openlocfilehash: ef194c045bfd2b416e382c12381afd68ba56dcf3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516691"
---
# <a name="hasirm"></a>HasIrm

**L’élément HasIrm** spécifie si au moins un message dans la conversation et le dossier actuel est un message protégé par IRM. 
  
```XML
<HasIrm> true | false </HasIrm>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Conversation (ConversationType)](conversation-conversationtype.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément HasIrm** est **true** si au moins un message de la conversation et le dossier en cours ont la gestion des erreurs. Sinon, la valeur est **false**.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Conversation (ConversationType)](conversation-conversationtype.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

