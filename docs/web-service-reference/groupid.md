---
title: GroupId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 656d9b9a-8a65-4a75-8466-5b0d96512dab
description: L’élément GroupId identifie de manière unique un groupe.
ms.openlocfilehash: eaba176321c0dd872b71ef50cbaa298d1277bb79
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827750"
---
# <a name="groupid"></a>GroupId

L’élément **GroupId** identifie de manière unique un groupe. 
  
```XML
<GroupId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |La valeur de texte de l’attribut **Id** est l’identificateur du groupe.  <br/> |
|ChangeKey  <br/> |La valeur de texte de l’attribut **ChangeKey** est la clé de modification du groupe.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[AddNewImContactToGroup](addnewimcontacttogroup.md) | [AddNewTelUriContactToGroup](addnewteluricontacttogroup.md) | [AddImContactToGroup](addimcontacttogroup.md) | [RemoveContactFromImList](removecontactfromimlist.md) | [RemoveImContactFromGroup](removeimcontactfromgroup.md) | [RemoveImGroup](removeimgroup.md)  |  [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md) | [SetImGroup](setimgroup.md)
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

