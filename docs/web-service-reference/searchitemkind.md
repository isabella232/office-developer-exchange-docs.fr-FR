---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: L’élément SearchItemKind indique le type d’éléments qui sont recherchées dans une opération FindMailboxStatisticsByKeyword.
ms.openlocfilehash: 1c099fc49ec882c1672b265ff0e3aa2c71c5f95b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829298"
---
# <a name="searchitemkind"></a>SearchItemKind

L’élément **SearchItemKind** indique le type d’éléments qui sont recherchées dans une opération **FindMailboxStatisticsByKeyword** . 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 **SearchItemKindType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[MessageTypes](messagetypes.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **SearchItemKind** est le type d’élément dans laquelle recherche des mots clés. La liste suivante contient les valeurs de texte qui peuvent être utilisés dans l’élément **SearchItemKind** . 
  
- **Courrier électronique** - indique que les messages électroniques sont exclus des mots clés. 
    
- **Réunions** - indique que les réunions sont exclues des mots clés. 
    
- **Tâches** - indique que les tâches sont exclus des mots clés. 
    
- **Notes** - indique que les notes sont exclus des mots clés. 
    
- **Documents** - indique que les documents sont exclus des mots clés. 
    
- **Feuilles** - indique que les journaux sont exclus des mots clés. 
    
- **Contacts** - indique que les contacts sont exclus des mots clés. 
    
- **Messagerie instantanée** - indique que les messages instantanés sont exclus des mots clés. 
    
- **Messagerie vocale** - indique que les messages vocaux sont exclus des mots clés. 
    
- **Télécopies** - indique que les télécopies sont exclus des mots clés. 
    
- **Billets** - indique que les billets sont recherchés des mots clés. 
    
- **Rssfeeds** - indique que les flux RSS sont exclus des mots clés. 
    
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

