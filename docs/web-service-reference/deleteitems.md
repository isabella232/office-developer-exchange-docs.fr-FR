---
title: DeleteItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItems
api_type:
- schema
ms.assetid: a5898bfc-f5ae-451d-9713-3e55864c690c
description: L’élément DeleteItems indique les éléments dans un dossier un utilisateur est autorisé à supprimer. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 0be2154d1ceb6a995df8b27033fdc59bca81f9ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755878"
---
# <a name="deleteitems"></a>DeleteItems

L’élément **DeleteItems** indique les éléments dans un dossier un utilisateur est autorisé à supprimer. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DeleteItems>None or Owned or All</DeleteItems>
```

 **PermissionActionType**
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
|[CalendarPermission](calendarpermission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **DeleteItems** . 
  
**Valeurs de texte des éléments DeleteItems**

|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |Indique que l’utilisateur n’est pas autorisé à supprimer des éléments dans le dossier.  <br/> |
|Propriétaire  <br/> |Indique que l’utilisateur est autorisé à supprimer les éléments qui appartiennent à l’utilisateur dans le dossier.  <br/> |
|Tous  <br/> |Indique que l’utilisateur est autorisé à supprimer tous les éléments dans le dossier.  <br/> |
   
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
- [Setting Folder-Level Permissions](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

