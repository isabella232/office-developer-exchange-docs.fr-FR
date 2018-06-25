---
title: Attribution (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: L’élément Attribution spécifie une instance d’un tableau d’attributs pour un élément PersonaType.
ms.openlocfilehash: 0e800c92c75bf0c475d4bffd33d6ab49f9ad9a9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755349"
---
# <a name="attribution-personaattributiontype"></a>Attribution (PersonaAttributionType)

L’élément **Attribution** spécifie une instance d’un tableau d’attributs pour un élément **PersonaType** . 
  
```XML
<Attribution>
    <Id></Id>
    <SourceId></SourceId>
    <DisplayName></DisplayName>
    <IsWritable></IsWritable>
    <IsQuickContact></IsQuickContact>
    <IsHidden></IsHidden>
    <FolderId></FolderId>
</Attribution>
```

 **PersonaAttributionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID (chaîne)](id-string.md) <br/> |Spécifie une chaîne qui identifie de manière unique une application ou une attribution dans un personnage.  <br/> |
|[ID source](sourceid.md) <br/> |Spécifie l’identificateur du contact ou du destinataire d’Active Directory.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Définit le nom complet d’un dossier, contact, liste de distribution, délégué utilisateur ou de règle.  <br/> |
|[IsWritable](iswritable.md) <br/> |Spécifie si l’ou les destinataires d’Active Directory sous-jacent peut être écrite.  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |Spécifie une valeur de type Boolean qui indique si l’ou les destinataires d’Active Directory sous-jacent est un contact rapide.  <br/> |
|[IsHidden](ishidden.md) <br/> |Contient une valeur de type Boolean qui indique si l’ou les destinataires d’Active Directory sous-jacent doit être masqué ou affiché dans le cadre du personnage.  <br/> |
|[FolderId](folderid.md) <br/> |Contient la clé d’identificateur et de modification d’un dossier.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |Spécifie un tableau des informations d’attribution d’un ou plusieurs contacts ou des destinataires d’active directory (AD) regroupées dans les personnages associés.  <br/> |
   
## <a name="remarks"></a>Remarques

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

