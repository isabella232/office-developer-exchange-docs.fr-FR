---
title: MaxChangesReturned
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MaxChangesReturned
api_type:
- schema
ms.assetid: f471db84-a666-4dfa-9993-8ca9113a0384
description: L’élément MaxChangesReturned décrit le nombre maximal de modifications qui peuvent être renvoyées dans une réponse de synchronisation.
ms.openlocfilehash: 8169e1a87ed22b68e5115cd7eaaa1084e44e8f33
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523932"
---
# <a name="maxchangesreturned"></a>MaxChangesReturned

**L’élément MaxChangesReturned** décrit le nombre maximal de modifications qui peuvent être renvoyées dans une réponse de synchronisation. 
  
[SyncFolderItems](syncfolderitems.md)
  
[MaxChangesReturned](maxchangesreturned.md)
  
```xml
<MaxChangesReturned/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |Définit une demande de synchronisation des éléments dans un Exchange de la boutique d’information.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente un nombre complet qui décrit le nombre maximal d’éléments renvoyés dans un seul appel de synchronisation. La valeur doit être entre 1 et 512 inclus.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

