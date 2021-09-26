---
title: StreamingSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StreamingSubscriptionRequest
api_type:
- schema
ms.assetid: d18f3b60-ebb6-4133-b895-a6ec8942d039
description: L’élément StreamingSubscriptionRequest représente un abonnement à un abonnement de notification d’événement de diffusion en continu.
ms.openlocfilehash: 9789329f3f59cb543861dca0232207669f0711b8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544548"
---
# <a name="streamingsubscriptionrequest"></a>StreamingSubscriptionRequest

**L’élément StreamingSubscriptionRequest** représente un abonnement à un abonnement de notification d’événement de diffusion en continu. 
  
[Subscribe](subscribe.md)
  
[StreamingSubscriptionRequest](streamingsubscriptionrequest.md)
  
```xml
<StreamingSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
</StreamingSubscriptionRequest>
```

 **StreamingSubscriptionRequest**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |Indique si le serveur s’abonnera à tous les dossiers de la boîte aux lettres de l’utilisateur. La valeur **true indique** que le serveur s’abonnera.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Contient un tableau d’identificateurs de dossiers utilisés pour identifier les dossiers à surveiller pour les notifications d’événement.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Contient une collection de notifications d’événements utilisées pour créer un abonnement.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Subscribe](subscribe.md) <br/> |Contient les propriétés utilisées pour créer des abonnements.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.Cet élément est une nouveauté d'Exchange Server 2010 Service Pack 1 (SP1).
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération d'abonnement](subscribe-operation.md)
  
[Opération de GetEvents](getevents-operation.md)
  
[Opération de GetStreamingEvents](getstreamingevents-operation.md)
  
[Opération de résiliation d'abonnement](unsubscribe-operation.md)

