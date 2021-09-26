---
title: SenderSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SenderSmtpAddress
api_type:
- schema
ms.assetid: e39c7df7-4bfa-455f-b4bb-1f1d05398eec
description: L’élément SenderSmtpAddress représente l’adresse de messagerie SMTP correspondant à la boîte aux lettres qui contient le dossier qui sera partagé.
ms.openlocfilehash: 09a0c577850581c7c67c6fff241a5d848421ed71
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546090"
---
# <a name="sendersmtpaddress"></a>SenderSmtpAddress

**L’élément SenderSmtpAddress** représente l’adresse de messagerie SMTP correspondant à la boîte aux lettres qui contient le dossier qui sera partagé. 
  
```xml
<SenderSmtpAddress/>
```

 **NonEmptyStringType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetSharingMetadata](getsharingmetadata.md) <br/> |Définit une demande d’obtenir un jeton d’authentification opaque qui identifie l’invitation de partage.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une adresse SMTP est requise.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur qui le rôle serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetSharingMetadata](getsharingmetadata-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

