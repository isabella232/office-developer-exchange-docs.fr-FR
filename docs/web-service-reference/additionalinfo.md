---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: L’élément AdditionalInfo spécifie des informations supplémentaires sur l’état de conservation d’une boîte aux lettres.
ms.openlocfilehash: 6fbe24d5d3e41f2ba9c81657b2c38240d10eefed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755173"
---
# <a name="additionalinfo"></a>AdditionalInfo

L’élément **AdditionalInfo** spécifie des informations supplémentaires sur l’état de conservation d’une boîte aux lettres. 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 **xs : String**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailboxHoldStatus](mailboxholdstatus.md) <br/> |Spécifie l’état de conservation de la boîte aux lettres.  <br/> |
|[NonIndexableItemDetail](nonindexableitemdetail.md) <br/> |Spécifie les détails d’un élément qui ne peuvent pas être indexé.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément AdditionalInfo est plus d’informations sur l’état de conservation d’une boîte aux lettres.
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

