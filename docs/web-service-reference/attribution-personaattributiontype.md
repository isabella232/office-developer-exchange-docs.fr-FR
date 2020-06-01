---
title: Attribution (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: L’élément spécifie une instance dans un tableau d’attributs pour un élément PersonaType.
ms.openlocfilehash: 05b0d41c116f2ed7b8dbb3ac44108bb879256b5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464174"
---
# <a name="attribution-personaattributiontype"></a>Attribution (PersonaAttributionType)

L' **élément** spécifie une instance dans un tableau d’attributs pour un élément **PersonaType** . 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ID (chaîne)](id-string.md) <br/> |Spécifie une chaîne qui identifie de manière unique une application ou une attribution dans un personnage.  <br/> |
|[SourceId](sourceid.md) <br/> |Spécifie l’identificateur du destinataire du contact ou Active Directory.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Définit le nom d’affichage d’un dossier, d’un contact, d’une liste de distribution, d’un utilisateur délégué ou d’une règle.  <br/> |
|[IsWritable](iswritable.md) <br/> |Indique si le contact sous-jacent ou le destinataire Active Directory peut être accessible en écriture.  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |Spécifie une valeur de type Boolean qui indique si le contact sous-jacent ou le destinataire Active Directory est un contact rapide.  <br/> |
|[IsHidden](ishidden.md) <br/> |Contient une valeur de type Boolean qui indique si le destinataire sous-jacent ou Active Directory doit être masqué ou affiché en tant que partie du personnage.  <br/> |
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de modification d’un dossier.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |Spécifie un tableau d’informations d’attribution pour un ou plusieurs contacts ou destinataires Active Directory (AD) rassemblés dans le personnage associé.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

