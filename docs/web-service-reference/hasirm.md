---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: L’élément HasIrm spécifie si au moins un message de la conversation et le dossier actif est un message protégé par IRM.
ms.openlocfilehash: 1596610ed5f6b2bac353900624fbec9140aaa693
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462779"
---
# <a name="hasirm"></a>HasIrm

L’élément **HasIrm** spécifie si au moins un message de la conversation et le dossier actif est un message protégé par IRM. 
  
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

La valeur de texte de l’élément **HasIrm** est **true** si au moins un message de la conversation et le dossier actif a une gestion des droits relatifs à l’information (IRM). Sinon, la valeur est **false**.
  
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

