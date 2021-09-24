---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: L’élément GlobalHasIrm spécifie si au moins un message dans la conversation et dans tous les dossiers est un message protégé par IRM.
ms.openlocfilehash: bd3414136a115b016c291fa0482682efcc7d9e1a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516831"
---
# <a name="globalhasirm"></a>GlobalHasIrm

**L’élément GlobalHasIrm** spécifie si au moins un message dans la conversation et dans tous les dossiers est un message protégé par IRM. 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
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

La valeur de texte de l’élément **GlobalHasIrm** est **true** si au moins un message dans la conversation et dans tous les dossiers est un message protégé par IRM. Sinon, la valeur est **false**.
  
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

