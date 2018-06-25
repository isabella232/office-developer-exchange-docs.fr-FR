---
title: TasksFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolderPermissionLevel
api_type:
- schema
ms.assetid: 0f70b79b-3443-4048-b410-692d4e2464fc
description: L’élément TasksFolderPermissionLevel contient les autorisations pour le dossier tâches par défaut. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 49807896f9175bafbef106c41d1c9dff8f6178c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838673"
---
# <a name="tasksfolderpermissionlevel"></a>TasksFolderPermissionLevel

L’élément **TasksFolderPermissionLevel** contient les autorisations pour le dossier tâches par défaut. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<TasksFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</TasksFolderPermissionLevel>
```

**DelegateFolderPermissionLevelType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DelegatePermissions](delegatepermissions.md) <br/> |Contient les paramètres au niveau d’autorisation délégué pour un utilisateur. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs de texte qui représentent les niveaux d’autorisation.
  
**Valeurs de texte de niveau d’autorisation**

|**Niveau d’autorisation**|**Description**|
|:-----|:-----|
|None  <br/> |L’utilisateur délégué a des autorisations d’accès au dossier tâches.  <br/> |
|Reviewer  <br/> |L’utilisateur délégué peut lire des éléments dans le dossier tâches.  <br/> |
|Auteur  <br/> |L’utilisateur délégué pouvant lire et créer des éléments dans le dossier tâches.  <br/> |
|Editor  <br/> |L’utilisateur délégué peut lire, créer et modifier des éléments dans le dossier tâches.  <br/> |
|Personnalisé  <br/> |L’utilisateur délégué dispose des autorisations d’accès personnalisé au dossier tâches.  <br/> |
   
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

- [Opération AddDelegate](adddelegate-operation.md)
- [Opération UpdateDelegate](updatedelegate-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Ajout de délégués](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

