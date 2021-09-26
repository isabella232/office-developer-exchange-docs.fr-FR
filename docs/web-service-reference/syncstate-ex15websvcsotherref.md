---
title: SyncState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncState
api_type:
- schema
ms.assetid: e5ebaae3-0f07-481d-ac67-d9687a3c7ac3
description: L’élément SyncState contient une forme codée en base 64 des données de synchronisation qui est mise à jour après chaque demande réussie. Il est utilisé pour identifier l’état de synchronisation.
ms.openlocfilehash: 72a0e347b5732cbe397956f8cc50b3266fba9156
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543904"
---
# <a name="syncstate"></a>SyncState

**L’élément SyncState** contient une forme codée en base 64 des données de synchronisation qui est mise à jour après chaque demande réussie. Il est utilisé pour identifier l’état de synchronisation. 
  
```xml
<SyncState/>
```

 **String**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SyncFolderHierarchy](syncfolderhierarchy.md) <br/> |Définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.  <br/> |
|[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande SyncFolderHierarchy.  <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Définit une demande de synchronisation des éléments dans un Exchange de la boutique d’information.  <br/> |
|[SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande SyncFolderItems.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise lorsque cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)
  
[Opération SyncFolderHierarchy](syncfolderhierarchy-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

