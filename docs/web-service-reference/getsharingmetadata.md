---
title: GetSharingMetadata
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadata
api_type:
- schema
ms.assetid: b609ee26-6d28-4559-81b6-b8e8d4759a23
description: L’élément GetSharingMetadata définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage. Cet élément est l’élément de base pour l’opération GetSharingMetadata.
ms.openlocfilehash: 5283d35e11350ef10ed8cc01527e787ef54be927
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827677"
---
# <a name="getsharingmetadata"></a>GetSharingMetadata

L’élément **GetSharingMetadata** définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage. Cet élément est l’élément de base pour l' [opération GetSharingMetadata](getsharingmetadata-operation.md).
  
```XML
<GetSharingMetadata>
   <IdOfFolderToShare/>
   <SenderSmtpAddress/>
   <Recipients/>
</GetSharingMetadata>
```

 **GetSharingMetadataType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[IdOfFolderToShare](idoffoldertoshare.md) <br/> |Représente l’identificateur du dossier sur le serveur qui est partagé. Cet élément est obligatoire.  <br/> |
|[SenderSmtpAddress](sendersmtpaddress.md) <br/> |Représente l’adresse de messagerie SMTP qui correspond à la boîte aux lettres qui contient le dossier identifié par l’élément [IdOfFolderToShare](idoffoldertoshare.md) . Cet élément est obligatoire.  <br/> |
|[Destinataires (ArrayOfSmtpAddressType)](recipients-arrayofsmtpaddresstype.md) <br/> |Représente les adresses de messagerie SMTP d’une ou plusieurs entités qui auront accès aux données dans le dossier identifié par l’élément [IdOfFolderToShare](idoffoldertoshare.md) . Cet élément est obligatoire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetSharingMetadata](getsharingmetadata-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

