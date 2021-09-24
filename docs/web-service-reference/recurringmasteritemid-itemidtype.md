---
title: RecurringMasterItemId (ItemIdType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 48d831cf-10d8-480b-86d2-f9c0b14b8167
description: L’élément RecurringMasterItemId (ItemIdType) identifie un élément maître de récurrence en identifiant les identificateurs de l’un de ses éléments d’occurrence associés.
ms.openlocfilehash: 491bb6686ad6cc9ee8169144b659d828e3920e45
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522739"
---
# <a name="recurringmasteritemid-itemidtype"></a>RecurringMasterItemId (ItemIdType)

**L’élément RecurringMasterItemId (ItemIdType)** identifie un élément maître de récurrence en identifiant les identificateurs de l’un de ses éléments d’occurrence connexes. 
  
```XML
<RecurringMasterItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

****

|**Attribut**|**Description**|
|:-----|:-----|
|ID  <br/> |Identifie une occurrence unique d’un élément principal périodique. Cet attribut est obligatoire.  <br/> |
|ChangeKey  <br/> |Identifie une version spécifique d’une occurrence unique d’un élément principal périodique. En outre, l’élément maître périodique est également identifié car il et l’occurrence unique contiendra la même touche de modification. Cet attribut est facultatif.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Reminder](reminder.md)
  
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



[Reminder](reminder.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

