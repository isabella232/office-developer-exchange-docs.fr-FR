---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: L’élément SyncScope indique si uniquement les éléments ou les éléments et les informations associées au dossier sont renvoyés dans une réponse de la synchronisation.
ms.openlocfilehash: 847c0244a8847364e29ea584b0c0b721f00d3064
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838666"
---
# <a name="syncscope"></a>SyncScope

L’élément **SyncScope** indique si uniquement les éléments ou les éléments et les informations associées au dossier sont renvoyés dans une réponse de la synchronisation. 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 **SyncFolderItemsScopeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SyncFolderItems](syncfolderitems.md) <br/> |L’élément qui définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/> / SyncFolderItems  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Le tableau suivant répertorie les valeurs possibles pour l’élément **SyncScope** . 
  
**Valeurs des éléments SyncScope**

|**Valeur**|**Description**|
|:-----|:-----|
|NormalItems  <br/> |Spécifie que seuls les éléments dans le dossier sont retournés dans une réponse de la synchronisation.  <br/> |
|NormalAndAssociatedItems  <br/> |Spécifie que les deux éléments dans le dossier et les informations associées au dossier sont retournés dans une réponse de la synchronisation.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

