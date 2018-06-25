---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: L’élément SyncFolderHierarchy définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.
ms.openlocfilehash: f72640e5605dd83e92cd323cb00e4d2f64406245
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838658"
---
# <a name="syncfolderhierarchy"></a>SyncFolderHierarchy

L’élément **SyncFolderHierarchy** définit une demande de synchronisation d’une hiérarchie de dossiers sur un client. 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 **SyncFolderHierarchyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifie les propriétés du dossier à inclure dans une réponse [SyncFolderHierarchy](syncfolderhierarchy.md) .  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Représente le dossier qui contient les éléments à synchroniser. Cet élément est facultatif.  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |Contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64. Il est utilisé pour identifier l’état de synchronisation.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
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



[Opération SyncFolderHierarchy](syncfolderhierarchy-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

