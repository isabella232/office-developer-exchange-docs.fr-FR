---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: L’élément ReadItems indique si un utilisateur est autorisé à lire des éléments dans un dossier Calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a12b5316eaebfdf6d0d70468f172f227db7ab3ef
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519085"
---
# <a name="readitems-calendarpermissiontype"></a>ReadItems (CalendarPermissionType)

**L’élément ReadItems** indique si un utilisateur est autorisé à lire des éléments dans un dossier Calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Le tableau suivant répertorie les valeurs possibles pour **l’élément ReadItems.** 
  
**Valeurs de texte de l’élément ReadItems**

|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Indique que l’utilisateur n’est pas autorisé à afficher les éléments du calendrier.  <br/> |
|TimeOnly  <br/> |Indique que l’utilisateur est autorisé à afficher uniquement les heures de libre/occupé dans le calendrier.  <br/> |
|TimeAndSubjectAndLocation  <br/> |Indique que l’utilisateur est autorisé à afficher les heures de libre/occupé dans le calendrier, ainsi que l’objet et l’emplacement des rendez-vous.  <br/> |
|FullDetails  <br/> |Indique que l’utilisateur est autorisé à afficher tous les éléments du calendrier, y compris les heures de libre/occupé et l’objet, l’emplacement et les détails des rendez-vous.  <br/> |
   
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

