---
title: UserOptions
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1acbb8a3-9110-4427-a06c-7e6e627e969f
description: L’élément UserOptions spécifie la liste des options de vote sur un message.
ms.openlocfilehash: 3f4a30cf66700210dc0a6bcce4d5d4521a288a7c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541692"
---
# <a name="useroptions"></a>UserOptions

**L’élément UserOptions** spécifie la liste des options de vote sur un message. 
  
```XML
<UserOptions>
   <VotingOptionData>
</UserOptions>
```

 **ArrayOfVotingOptionDataType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[VotingOptionData](votingoptiondata.md)
  
### <a name="parent-elements"></a>Éléments parents

[VotingInformation](votinginformation.md)
  
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



[VotingInformation](votinginformation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

