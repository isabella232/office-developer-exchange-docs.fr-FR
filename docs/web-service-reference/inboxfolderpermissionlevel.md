---
title: InboxFolderPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- InboxFolderPermissionLevel
api_type:
- schema
ms.assetid: f250d31b-9193-4c1c-8350-900dead3a023
description: L’élément InboxFolderPermissionLevel contient les autorisations pour le dossier boîte de réception par défaut. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 33db919e3f19ab567ea53386d11afeace58bd213
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515676"
---
# <a name="inboxfolderpermissionlevel"></a>InboxFolderPermissionLevel

**L’élément InboxFolderPermissionLevel** contient les autorisations pour le dossier boîte de réception par défaut. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<InboxFolderPermissionLevel>
   None or Editor or Reviewer or Author or Custom
</InboxFolderPermissionLevel>
```

 **DelegateFolderPermissionLevelType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DelegatePermissions](delegatepermissions.md) <br/> |Contient les paramètres de niveau d’autorisation délégué pour un utilisateur. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs de texte qui représentent les niveaux d’autorisation.
  
**Valeurs de texte de niveau d’autorisation**

|**Niveau d’autorisation**|**Description**|
|:-----|:-----|
|Aucun  <br/> |L’utilisateur délégué n’a aucune autorisation d’accès au dossier Boîte de réception.  <br/> |
|Relecteur  <br/> |L’utilisateur délégué peut lire les éléments du dossier Boîte de réception.  <br/> |
|Auteur  <br/> |L’utilisateur délégué peut lire et créer des éléments dans le dossier Boîte de réception.  <br/> |
|Éditeur  <br/> |L’utilisateur délégué peut lire, créer et modifier des éléments dans le dossier Boîte de réception.  <br/> |
|Personnalisé  <br/> |L’utilisateur délégué dispose d’autorisations d’accès personnalisées au dossier Boîte de réception.  <br/> |
   
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



[Opération AddDelegate](adddelegate-operation.md)
  
[Opération UpdateDelegate](updatedelegate-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)


[Ajout de délégués](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

