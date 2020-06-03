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
description: L’élément SyncFolderItems définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.
ms.openlocfilehash: 0fa5b1544d5627d1423287369e72f97662c28d12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465148"
---
# <a name="syncfolderitems"></a>SyncFolderItems

L’élément **SyncFolderItems** définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ItemShape](itemshape.md) <br/> |Identifie les propriétés d’élément et le contenu à inclure dans une réponse SyncFolderItems. Cet élément est obligatoire.  <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Représente le dossier qui contient les éléments à synchroniser. Cet élément est obligatoire.  <br/> |
|[SyncState](syncstate-ex15websvcsotherref.md) <br/> |Contient un formulaire codé en base64 des données de synchronisation qui sont mises à jour après chaque demande réussie. Il est utilisé pour identifier l’état de synchronisation. Cet élément est facultatif.  <br/> |
|[Ignore](ignore.md) <br/> |Identifie les éléments à ignorer lors de la synchronisation. Cet élément est facultatif.  <br/> |
|[MaxChangesReturned](maxchangesreturned.md) <br/> |Décrit le nombre maximal de modifications pouvant être renvoyées dans une réponse de synchronisation. Cet élément est obligatoire.  <br/> |
|[SyncScope](syncscope.md) <br/> |Indique si les éléments ou les éléments et les informations associés uniquement sont renvoyés dans une réponse de synchronisation. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |schéma des messages  <br/> |
|Fichier de validation  <br/> |messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

