---
title: ApprovalRequestData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6c971cf7-5c3a-4e5e-9a7d-048f4ac0aadb
description: L’élément ApprovalRequestData spécifie l’état d’approbation d’un message de demande d’approbation.
ms.openlocfilehash: decbd4d646a56b9810387adcdb6a9049da89bc38
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462303"
---
# <a name="approvalrequestdata"></a>ApprovalRequestData

L’élément **ApprovalRequestData** spécifie l’état d’approbation d’un message de demande d’approbation. 
  
```xml
<ApprovalRequestData>
   <IsUndecidedApprovalRequest/>
   <ApprovalDecision/>
   <ApprovalDecisionMaker/>
   <ApprovalDecisionTime/>
</ApprovalRequestData>
```

 **ApprovalRequestDataType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

[IsUndecidedApprovalRequest](isundecidedapprovalrequest.md)  |  [ApprovalDecision](approvaldecision.md)  |  [ApprovalDecisionMaker](approvaldecisionmaker.md)  |  [ApprovalDecisionTime](approvaldecisiontime.md)
  
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

- [Message](message-ex15websvcsotherref.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

