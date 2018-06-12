---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: L’élément SendPrompt Spécifie le type d’action pour une option de vote.
ms.openlocfilehash: f3220d957482ea04c46b014cdf1c67025d5ec21a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829346"
---
# <a name="sendprompt"></a>SendPrompt

L’élément **SendPrompt** Spécifie le type d’action pour une option de vote. 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 **SendPromptType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[VotingOptionData](votingoptiondata.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **SendPrompt** est une action option vote. Le tableau suivant répertorie les valeurs possibles de cet élément. 
  
****

|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |Aucune action.  <br/> |
|Envoyer  <br/> |La réponse est envoyée immédiatement.  <br/> |
|VotingOption  <br/> |L’approbateur peut entrer des commentaires lors de l’approbation ou rejet.  <br/> |
   
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



[VotingOptionData](votingoptiondata.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

