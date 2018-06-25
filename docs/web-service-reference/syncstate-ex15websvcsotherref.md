---
title: SyncState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncState
api_type:
- schema
ms.assetid: e5ebaae3-0f07-481d-ac67-d9687a3c7ac3
description: L’élément SyncState contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64. Il est utilisé pour identifier l’état de synchronisation.
ms.openlocfilehash: 3c600dde09fd813dcfb1f6e74671ebe9004701a1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838667"
---
# <a name="syncstate"></a>SyncState

L’élément **SyncState** contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64. Il est utilisé pour identifier l’état de synchronisation. 
  
```xml
<SyncState/>
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
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |Définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande SyncFolderHierarchy.  <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande SyncFolderItems.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte est requise lorsque cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)
  
[Opération SyncFolderHierarchy](syncfolderhierarchy-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

