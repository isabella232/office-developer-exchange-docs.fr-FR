---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: L’élément SearchItemKind indique le type d’éléments recherchés pour une opération FindMailboxStatisticsByKeyword.
ms.openlocfilehash: 93803d181f32d88c30ab0fa9a72bb92f22907dde
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510854"
---
# <a name="searchitemkind"></a>SearchItemKind

**L’élément SearchItemKind** indique le type d’éléments recherchés pour une opération **FindMailboxStatisticsByKeyword.** 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 **SearchItemKindType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[MessageTypes](messagetypes.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément SearchItemKind** est le type d’élément recherché pour les mots clés. La liste suivante contient les valeurs de texte qui peuvent être utilisées dans **l’élément SearchItemKind.** 
  
- **Courrier** électronique : indique que des mots clés sont recherchés dans les messages électroniques. 
    
- **Réunions :** indique que des mots clés sont recherchés dans les réunions. 
    
- **Tâches** : indique que des mots clés sont recherchés dans les tâches. 
    
- **Remarques** : indique que des mots clés sont recherchés dans les notes. 
    
- **Documents :** indique que des mots clés sont recherchés dans les documents. 
    
- **Journaux** : indique que des mots clés sont recherchés dans les journaux. 
    
- **Contacts** : indique que des mots clés sont recherchés dans les contacts. 
    
- **Messagerie** instantanée : indique que des mots clés sont recherchés dans les messages instantanés. 
    
- **Messagerie vocale** : indique que les messages vocaux sont recherchés à la recherche de mots clés. 
    
- **Télécopies** : indique que des mots clés sont recherchés pour les télécopies. 
    
- **Publications** : indique que les billets sont recherchés pour des mots clés. 
    
- **Flux Rss :** indique que les flux RSS sont recherchés pour des mots clés. 
    
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

