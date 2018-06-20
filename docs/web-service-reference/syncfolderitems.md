---
title: SyncFolderItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItems
api_type:
- schema
ms.assetid: 463ed78c-bf82-4cd8-971a-d18425e9e7be
description: L’élément SyncFolderItems définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.
ms.openlocfilehash: 368e19babfccaeab40380103495c63d30647905c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838662"
---
# <a name="syncfolderitems"></a>SyncFolderItems

L’élément **SyncFolderItems** définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange. 
  
```xml
<SyncFolderItems>
   <ItemShape/>
   <SyncFolderId/>
   <SyncState/>
   <Ignore/>
   <MaxChangesReturned/>   <SyncScope/>
</SyncFolderItems>
```

 **SyncFolderItemsType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifie les propriétés de l’élément et le contenu à inclure dans une réponse SyncFolderItems. Cet élément est obligatoire.  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Représente le dossier qui contient les éléments à synchroniser. Cet élément est obligatoire.  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |Contient un formulaire de la synchronisation de données est mis à jour après chaque requête réussie codé en base64. Il est utilisé pour identifier l’état de synchronisation. Cet élément est facultatif.  <br/> |
|[Ignorer](ignore.md) <br/> |Identifie les éléments à ignorer lors de la synchronisation. Cet élément est facultatif.  <br/> |
|[MaxChangesReturned](maxchangesreturned.md) <br/> |Indique le nombre maximal de modifications pouvant être renvoyés dans une réponse de la synchronisation. Cet élément est obligatoire.  <br/> |
|[SyncScope](syncscope.md) <br/> |Indique si seulement les éléments ou les éléments et les informations associées au dossier sont renvoyés dans une réponse de la synchronisation. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

