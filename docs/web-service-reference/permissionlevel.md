---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: L’élément PermissionLevel représente le niveau d’autorisation dont dispose un utilisateur sur un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 7cc734f5807fe039467065315c220341f47d3fb4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828730"
---
# <a name="permissionlevel"></a>PermissionLevel

L’élément **PermissionLevel** représente le niveau d’autorisation dont dispose un utilisateur sur un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 **PermissionLevelType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Autorisation](permission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **PermissionLevel** . 
  
**Valeurs de texte des éléments PermissionLevel**

|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |Indique que l’utilisateur n’a aucune autorisation sur le dossier.  <br/> |
|Owner  <br/> |Indique que l’utilisateur peut créer, lire, modifier, supprimer tous les éléments dans le dossier et créer des sous-dossiers. L’utilisateur est propriétaire du dossier et contact du dossier.  <br/> |
|Détenir  <br/> |Indique que l’utilisateur peut créer, lire, modifier, supprimer tous les éléments dans le dossier et créer des sous-dossiers.  <br/> |
|Editor  <br/> |Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments dans le dossier.  <br/> |
|PublishingAuthor  <br/> |Indique que l’utilisateur peut créer et lire tous les éléments dans le dossier, modifier et supprimer uniquement les éléments créés par l’utilisateur et créer des sous-dossiers.  <br/> |
|Auteur  <br/> |Indique que l’utilisateur peut créer et lire tous les éléments dans le dossier, modifier et supprimer uniquement les éléments créés par l’utilisateur.  <br/> |
|NoneditingAuthor  <br/> |Indique que l’utilisateur peut créer et lire tous les éléments dans le dossier et supprimer uniquement les éléments créés par l’utilisateur.  <br/> |
|Reviewer  <br/> |Indique que l’utilisateur peut lire tous les éléments dans le dossier.  <br/> |
|Collaborateur  <br/> |Indique que l’utilisateur peut créer des éléments dans le dossier. Le contenu du dossier n’apparaître pas.  <br/> |
|Personnalisé  <br/> |Indique que l’utilisateur dispose des autorisations d’accès personnalisées sur le dossier.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

