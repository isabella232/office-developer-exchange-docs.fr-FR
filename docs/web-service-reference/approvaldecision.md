---
title: ApprovalDecision
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e7c5687-cb9e-4f0b-ac8f-b82591914a39
description: L’élément ApprovalDecision spécifie la décision sur un message de demande d’approbation.
ms.openlocfilehash: 4ca73813440200e5d2fb9f920d81459d8cd5e4ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755305"
---
# <a name="approvaldecision"></a>ApprovalDecision

L’élément **ApprovalDecision** spécifie la décision sur un message de demande d’approbation. 
  
```XML
<ApprovalDecision> 1 | 2 </ApprovalDecision>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[ApprovalRequestData](approvalrequestdata.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **ApprovalDecision** est 1 si approuvé et 2 si rejeté. 
  
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

- [ApprovalRequestData](approvalrequestdata.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

