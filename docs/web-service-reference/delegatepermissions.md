---
title: DelegatePermissions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegatePermissions
api_type:
- schema
ms.assetid: 292badc7-bab3-4368-9d7c-9a8b7edb279b
description: L’élément DelegatePermissions contient les paramètres de niveau d’autorisation de délégué pour un utilisateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 319592b6c3386a07b3094115c335c7fb8ffe1130
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755834"
---
# <a name="delegatepermissions"></a>DelegatePermissions

L’élément **DelegatePermissions** contient les paramètres de niveau d’autorisation de délégué pour un utilisateur. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DelegatePermissions>
   <CalendarFolderPermissionLevel/>
   <TasksFolderPermissionLevel/>
   <InboxFolderPermissionLevel/>
   <ContactsFolderPermissionLevel/>
   <NotesFolderPermissionLevel/>
   <JournalFolderPermissionLevel/>
</DelegatePermissions>
```

**DelegatePermissionsType**

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarFolderPermissionLevel](calendarfolderpermissionlevel.md) <br/> |Contient les autorisations pour le dossier calendrier par défaut. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[TasksFolderPermissionLevel](tasksfolderpermissionlevel.md) <br/> |Contient les autorisations pour le dossier tâches par défaut. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[InboxFolderPermissionLevel](inboxfolderpermissionlevel.md) <br/> |Contient les autorisations pour le dossier boîte de réception par défaut. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[ContactsFolderPermissionLevel](contactsfolderpermissionlevel.md) <br/> |Contient les autorisations pour le dossier Contacts par défaut. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[NotesFolderPermissionLevel](notesfolderpermissionlevel.md) <br/> |Contient les autorisations pour le dossier Notes par défaut. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
|[JournalFolderPermissionLevel](journalfolderpermissionlevel.md) <br/> |Contient les autorisations pour le dossier de Journal par défaut. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Utilisateur_délégué](delegateuser.md) <br/> |Identifie un délégué pour ajouter ou mettre à jour dans une boîte aux lettres unique. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
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

