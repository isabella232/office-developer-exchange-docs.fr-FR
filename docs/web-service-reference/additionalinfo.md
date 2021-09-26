---
title: AdditionalInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 50bebbab-2fef-4a27-a5a9-32d7200820b6
description: L’élément AdditionalInfo spécifie des informations supplémentaires sur l’état de la boîte aux lettres.
ms.openlocfilehash: d8b707fb04ffe91d5c7aa793c6b56c8bb048f160
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544317"
---
# <a name="additionalinfo"></a>AdditionalInfo

**L’élément AdditionalInfo** spécifie des informations supplémentaires sur l’état de la boîte aux lettres. 
  
```XML
<AdditionalInfo></AdditionalInfo>
```

 **xs:string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[MailboxHoldStatus](mailboxholdstatus.md) <br/> |Spécifie l’état de la boîte aux lettres en attente.  <br/> |
|[NonIndexableItemDetail](nonindexableitemdetail.md) <br/> |Spécifie le détail d’un élément qui ne peut pas être indexé.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte de l’élément AdditionalInfo est une information supplémentaire sur l’état de la boîte aux lettres de la boîte aux lettres.
  
## <a name="remarks"></a>Remarques

Cet élément est facultatif.
  
Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

