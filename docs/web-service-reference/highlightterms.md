---
title: HighlightTerms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ce4a2978-fd0c-41a4-ae65-aa6f5dc9a0f9
description: L’élément HighlightTerms identifie les termes surlignés renvoyés dans une opération FindItem et une réponse d’opération FindConversation.
ms.openlocfilehash: c55ffc010dc0cfb09403433aaf8a0809a26f71a3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457633"
---
# <a name="highlightterms"></a>HighlightTerms

L’élément **HighlightTerms** identifie les termes surlignés renvoyés dans une opération **FindItem** et une réponse d’opération **FindConversation** . 
  
```XML
<HighlightTerms>
   <Term/>
</HighlightTerms>
```

 **ArrayOfHighlightTermsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Terme
  
### <a name="parent-elements"></a>Éléments parents

[FindConversationResponse](findconversationresponse.md)  |  [FindItemResponseMessage](finditemresponsemessage.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> ||
   

