---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: L’élément PermissionLevel représente le niveau d’autorisation d’un utilisateur sur un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 48b8db48afe6ced137acceeade2911a044298d75
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544835"
---
# <a name="permissionlevel"></a>PermissionLevel

**L’élément PermissionLevel** représente le niveau d’autorisation d’un utilisateur sur un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 **PermissionLevelType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Autorisation](permission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément PermissionLevel.** 
  
**Valeurs de texte de l’élément PermissionLevel**

|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Indique que l’utilisateur n’a pas d’autorisations sur le dossier.  <br/> |
|Propriétaire  <br/> |Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments du dossier, et créer des sous-dossiers. L’utilisateur est à la fois le propriétaire du dossier et le contact du dossier.  <br/> |
|PublishingEditor  <br/> |Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments du dossier, et créer des sous-dossiers.  <br/> |
|Éditeur  <br/> |Indique que l’utilisateur peut créer, lire, modifier et supprimer tous les éléments du dossier.  <br/> |
|PublishingAuthor  <br/> |Indique que l’utilisateur peut créer et lire tous les éléments du dossier, modifier et supprimer uniquement les éléments créés par l’utilisateur et créer des sous-dossiers.  <br/> |
|Auteur  <br/> |Indique que l’utilisateur peut créer et lire tous les éléments du dossier, et modifier et supprimer uniquement les éléments créés par l’utilisateur.  <br/> |
|NoneditingAuthor  <br/> |Indique que l’utilisateur peut créer et lire tous les éléments du dossier et supprimer uniquement les éléments créés par l’utilisateur.  <br/> |
|Relecteur  <br/> |Indique que l’utilisateur peut lire tous les éléments du dossier.  <br/> |
|Collaborateur  <br/> |Indique que l’utilisateur peut créer des éléments dans le dossier. Le contenu du dossier n’apparaît pas.  <br/> |
|Personnalisé  <br/> |Indique que l’utilisateur dispose d’autorisations d’accès personnalisées sur le dossier.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

