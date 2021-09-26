---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: L’élément VotingInformation spécifie les informations de vote sur un message de vote et un message de demande d’approbation oùApproveandReject sont les options de vote.
ms.openlocfilehash: 7e5aedddbfe97bba935aa56b3583e2fb8b081320
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543855"
---
# <a name="votinginformation"></a>VotingInformation

**L’élément VotingInformation** spécifie les informations de vote sur un message de vote et un message de demande d’approbation où « Approuver » et « Rejeter » sont les options de vote. 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 **VotingInformationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[UserOptions](useroptions.md)  |  [VotingResponse](votingresponse.md)
  
### <a name="parent-elements"></a>Éléments parents

[Message](message-ex15websvcsotherref.md)
  
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



[Message](message-ex15websvcsotherref.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

