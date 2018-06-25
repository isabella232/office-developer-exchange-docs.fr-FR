---
title: DisplayName (chaîne)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisplayName
api_type:
- schema
ms.assetid: e7efbbe1-6629-4d11-bed1-ed899e3f9d77
description: L’élément DisplayName définit le nom complet d’un dossier, contact, liste de distribution, délégué utilisateur, emplacement ou règle.
ms.openlocfilehash: 53f4e083d9e6617206e383d4408e08ed7ea0fe08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755990"
---
# <a name="displayname-string"></a>DisplayName (chaîne)

L’élément **DisplayName** définit le nom complet d’un dossier, contact, liste de distribution, délégué utilisateur, emplacement ou règle. 
  
```XML
<DisplayName/>
```

 **Chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Représente un dossier de calendrier dans une boîte aux lettres.  <br/> |
|[Contact](contact.md) <br/> |Représente un élément de contact Exchange.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Représente un dossier de contacts dans une boîte aux lettres.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Représente une liste de distribution.  <br/> |
|[Folder](folder.md) <br/> |Représente un dossier dans une boîte aux lettres.  <br/> |
|[Règle (RuleType)](rule-ruletype.md) <br/> |Représente une règle de boîte aux lettres d’un utilisateur.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Représente un dossier de recherche dans une boîte aux lettres.  <br/> |
|[Dossier tâches](tasksfolder.md) <br/> |Représente un dossier de tâches dans une boîte aux lettres.  <br/> |
|[Nom d’utilisateur](userid.md) <br/> |Identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte qui représente le nom complet est obligatoire si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="example"></a>Exemple

L’exemple suivant montre comment créer un nouveau dossier et la valeur DisplayName du dossier à « TestFolder ».
  
```cs
FolderType folder = new FolderType();
folder.DisplayName = "TestFolder";
```

## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

