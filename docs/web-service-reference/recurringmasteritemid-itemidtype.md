---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: L’élément RecurringMasterItemId (ItemIdType) identifie un élément de gabarit périodicité en identifiant les identificateurs de l’un de ses éléments connexes occurrence.
ms.openlocfilehash: 89089067963e99ac1a6cae6ea6e1e8350d148e82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829010"
---
# <a name="recurringmasteritemid-itemidtype"></a>RecurringMasterItemId (ItemIdType)

L’élément **RecurringMasterItemId (ItemIdType)** identifie un élément de gabarit périodicité en identifiant les identificateurs de l’un de ses éléments connexes occurrence. 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

****

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Identifie une seule occurrence d’un rendez-vous périodique. Cet attribut est requis.  <br/> |
|ChangeKey  <br/> |Identifie une version spécifique d’une seule occurrence d’un rendez-vous périodique. En outre, le rendez-vous périodique est également identifié, car elle et l’occurrence contiendra la même clé change. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Rappel](reminder.md)
  
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



[Rappel](reminder.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

