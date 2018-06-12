---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: L’élément IsUndecidedApprovalRequest Spécifie si un message de demande d’approbation a été effectuée.
ms.openlocfilehash: 82b4624df5b2fe7ca212fdf76248e1ccfa3a081f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828127"
---
# <a name="isundecidedapprovalrequest"></a>IsUndecidedApprovalRequest

L’élément **IsUndecidedApprovalRequest** Spécifie si un message de demande d’approbation a été effectuée. 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ApprovalRequestData](approvalrequestdata.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **IsUndecidedApprovalRequest** est **la valeur true** si un message de demande d’approbation n’a pas été effectuée. La valeur **false** indique que la demande d’approbation a été décidée. 
  
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



[ApprovalRequestData](approvalrequestdata.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

