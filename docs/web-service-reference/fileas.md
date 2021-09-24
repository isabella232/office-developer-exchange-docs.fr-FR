---
title: FileAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FileAs
api_type:
- schema
ms.assetid: df50524e-471c-49d2-89fe-b2d0f61a1365
description: L’élément FileAs représente le classement d’un contact ou d’une liste de distribution dans le dossier Contacts.
ms.openlocfilehash: 1ebed8365396feb42f4bfceac646ae7692dd6579
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530575"
---
# <a name="fileas"></a>FileAs

**L’élément FileAs représente** le classement d’un contact ou d’une liste de distribution dans le dossier Contacts. 
  
```xml
<FileAs/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une chaîne est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

**L’élément FileAs est** utilisé pour trier les contacts et les listes de distribution par un nom autre qu’un nom complet ou un nom de société. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

