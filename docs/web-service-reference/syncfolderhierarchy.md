---
title: SyncFolderHierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: 55df4d01-e48e-4263-a851-78a66ad1093a
description: L’élément SyncFolderHierarchy définit une demande de synchronisation d’une hiérarchie de dossiers sur un client.
ms.openlocfilehash: ebe8ecd613fee02275326be6377544959f85afb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531513"
---
# <a name="syncfolderhierarchy"></a>SyncFolderHierarchy

**L’élément SyncFolderHierarchy** définit une demande de synchronisation d’une hiérarchie de dossiers sur un client. 
  
```xml
<SyncFolderHierarchy>
   <FolderShape/>   <SyncFolderId/>
   <SyncState/>
</SyncFolderHierarchy>
```

 **SyncFolderHierarchyType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderShape](foldershape.md) <br/> |Identifie les propriétés de dossier à inclure dans une [réponse SyncFolderHierarchy.](syncfolderhierarchy.md)  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Représente le dossier qui contient les éléments à synchroniser. Cet élément est facultatif.  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |Contient une forme codée en base 64 des données de synchronisation qui est mise à jour après chaque demande réussie. Il est utilisé pour identifier l’état de synchronisation.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
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



[Opération SyncFolderHierarchy](syncfolderhierarchy-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

