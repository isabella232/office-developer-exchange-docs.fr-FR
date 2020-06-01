---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: L’élément SendPrompt spécifie le type d’action autorisé pour une option de vote.
ms.openlocfilehash: 98ffc69cdc94c3f7b9c325bee0c1ebaeb407ee96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462100"
---
# <a name="sendprompt"></a>SendPrompt

L’élément **SendPrompt** spécifie le type d’action autorisé pour une option de vote. 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 **SendPromptType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[VotingOptionData](votingoptiondata.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **SendPrompt** est une action d’option de vote. Le tableau suivant répertorie les valeurs possibles pour cet élément. 
  
****

|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Aucune action.  <br/> |
|Envoyer  <br/> |La réponse est envoyée immédiatement.  <br/> |
|VotingOption  <br/> |L’approbateur peut entrer des commentaires lors de l’approbation ou du rejet.  <br/> |
   
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



[VotingOptionData](votingoptiondata.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

