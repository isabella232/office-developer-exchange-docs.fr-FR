---
title: ReadItems (CalendarPermissionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReadItems
api_type:
- schema
ms.assetid: bec01982-26a1-4373-b1e6-2e0c838d83c4
description: L’élément ReadItems indique si un utilisateur est autorisé à lire les éléments dans un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 532b90c47cca7117a89d59e7012436268be9ebb0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828964"
---
# <a name="readitems-calendarpermissiontype"></a>ReadItems (CalendarPermissionType)

L’élément **ReadItems** indique si un utilisateur est autorisé à lire les éléments dans un dossier de calendrier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<ReadItems>None or TimeOnly or TimeAndSubjectAndLocation or FullDetails</ReadItems>
```

 **CalendarPermissionReadAccessType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **ReadItems** . 
  
**Valeurs de texte des éléments ReadItems**

|**Valeur**|**Description**|
|:-----|:-----|
|None  <br/> |Indique que l’utilisateur ne dispose pas d’autorisation d’afficher des éléments dans le calendrier.  <br/> |
|TimeOnly  <br/> |Indique que l’utilisateur est autorisé à afficher uniquement formulées dans le calendrier.  <br/> |
|TimeAndSubjectAndLocation  <br/> |Indique que l’utilisateur est autorisé à afficher le temps de disponibilité dans le calendrier et le sujet et l’emplacement du rendez-vous.  <br/> |
|FullDetails  <br/> |Indique que l’utilisateur est autorisé à afficher tous les éléments dans le calendrier, notamment formulées et subject, emplacement et les détails des rendez-vous.  <br/> |
   
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

