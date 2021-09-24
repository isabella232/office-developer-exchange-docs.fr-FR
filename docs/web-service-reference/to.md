---
title: À
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: L’élément To spécifie la cible de la transition de fuseau horaire. La cible est une période de fuseau horaire ou un groupe de transitions de fuseau horaire.
ms.openlocfilehash: 64f3f3258fd7c2bad051eabb1b33617bb056ab39
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522550"
---
# <a name="to"></a>À

**L’élément To** spécifie la cible de la transition de fuseau horaire. La cible est une période de fuseau horaire ou un groupe de transitions de fuseau horaire. 
  
```xml
<To Kind=""/>
```

 **TransitionTargetType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|Kind  <br/> |Indique si la cible de transition de fuseau horaire est une période de fuseau horaire ou d’un groupe de transitions de fuseau horaire.  <br/> |
   
#### <a name="kind-attribute-values"></a>Valeurs d’attribut kind

|**Valeur**|**Description**|
|:-----|:-----|
|Period  <br/> |Spécifie que la cible de transition de fuseau horaire est une période de fuseau horaire.  <br/> |
|Group  <br/> |Spécifie que la cible de transition de fuseau horaire est un groupe de transitions de fuseau horaire.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |Représente une transition de fuseau horaire qui se produit à une date et à une heure spécifiques.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Représente une transition de fuseau horaire qui se produit le même jour chaque année.  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Représente une transition de fuseau horaire qui se produit un jour de l’année spécifié.  <br/> |
|[Transition](transition.md) <br/> |Représente une transition de fuseau horaire.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte est une chaîne qui spécifie l’identificateur unique de period [ou](period.md) [transitionsGroup](transitionsgroup.md) qui est la cible de la transition de fuseau horaire. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

