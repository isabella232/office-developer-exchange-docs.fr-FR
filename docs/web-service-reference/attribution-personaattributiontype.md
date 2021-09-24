---
title: Attribution (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: L’élément Attribution spécifie une instance dans un tableau d’attributs pour un élément PersonaType.
ms.openlocfilehash: eb2fe66042b6c7f52732be20195f0f4b94ab867c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524377"
---
# <a name="attribution-personaattributiontype"></a>Attribution (PersonaAttributionType)

**L’élément Attribution** spécifie une instance dans un tableau d’attributs pour **un élément PersonaType.** 
  
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
|[ID (String)](id-string.md) <br/> |Spécifie une chaîne qui identifie de manière unique une application ou une attribution dans un personnage.  <br/> |
|[SourceId](sourceid.md) <br/> |Spécifie l’identificateur du contact ou du destinataire Active Directory.  <br/> |
|[DisplayName (chaîne)](displayname-string.md) <br/> |Définit le nom complet d’un dossier, d’un contact, d’une liste de distribution, d’un utilisateur délégué ou d’une règle.  <br/> |
|[IsWritable](iswritable.md) <br/> |Spécifie si le contact sous-jacent ou le destinataire Active Directory peut être écrit.  <br/> |
|[IsQuickContact](isquickcontact.md) <br/> |Spécifie une valeur de booléen qui indique si le contact sous-jacent ou le destinataire Active Directory est un contact rapide.  <br/> |
|[IsHidden](ishidden.md) <br/> |Contient une valeur boolé générale qui indique si le contact sous-jacent ou le destinataire Active Directory doit être masqué ou affiché dans le cadre du personnage.  <br/> |
|[FolderId](folderid.md) <br/> |Contient l’identificateur et la clé de modification d’un dossier.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Attributions (ArrayOfPersonaAttributionsType)](attributions-arrayofpersonaattributionstype.md) <br/> |Spécifie un tableau d’informations d’attribution pour un ou plusieurs des contacts ou des destinataires Active Directory (AD) agrégés dans le personnage associé.  <br/> |
   
## <a name="remarks"></a>Remarques

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

