---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: L’élément IsUndecidedApprovalRequest spécifie si un message de demande d’approbation a été pris en compte.
ms.openlocfilehash: 5204793490015bd2999322c0f029445c7df91e02
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511412"
---
# <a name="isundecidedapprovalrequest"></a>IsUndecidedApprovalRequest

**L’élément IsUndecidedApprovalRequest** spécifie si un message de demande d’approbation a été pris en compte. 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ApprovalRequestData](approvalrequestdata.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **IsUndecidedApprovalRequest** est **true** si un message de demande d’approbation n’a pas été pris en compte. La valeur **false indique** que la demande d’approbation a été décidée. 
  
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



[ApprovalRequestData](approvalrequestdata.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

