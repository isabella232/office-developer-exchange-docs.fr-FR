---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: L’élément SearchItemKind indique le type d’éléments recherchés pour une opération FindMailboxStatisticsByKeyword.
ms.openlocfilehash: e0625ac169c3083702494c094da15d38d220fe67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463999"
---
# <a name="searchitemkind"></a>SearchItemKind

L’élément **SearchItemKind** indique le type d’éléments recherchés pour une opération **FindMailboxStatisticsByKeyword** . 
  
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

La valeur de texte de l’élément **SearchItemKind** est le type d’élément qui fait l’objet de recherches de mots clés. La liste suivante contient les valeurs de texte qui peuvent être utilisées dans l’élément **SearchItemKind** . 
  
- **Email** : indique que les messages électroniques font l’objet de recherches de mots clés. 
    
- **Réunions** : indique que des mots clés sont recherchés dans les réunions. 
    
- **Tasks** : indique que les tâches font l’objet de recherches de mots clés. 
    
- **Remarques** : indique que des mots clés sont recherchés dans les notes. 
    
- **Docs** : indique que des mots clés sont recherchés dans les documents. 
    
- **Feuilles** : indique que les journaux font l’objet de recherches de mots clés. 
    
- **Contacts** : indique que des mots clés sont recherchés dans les contacts. 
    
- **Im** : indique que des mots clés sont recherchés dans les messages instantanés. 
    
- **Messagerie vocale** : indique que les messages vocaux font l’objet de recherches de mots clés. 
    
- **Télécopies** : indique que des mots clés sont recherchés dans les télécopies. 
    
- **Publications** : indique que des mots clés sont recherchés dans les publications. 
    
- **RSSFeeds** : indique que les flux RSS font l’objet de recherches de mots clés. 
    
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
   

