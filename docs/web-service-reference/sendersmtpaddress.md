---
title: SenderSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SenderSmtpAddress
api_type:
- schema
ms.assetid: e39c7df7-4bfa-455f-b4bb-1f1d05398eec
description: L’élément SenderSmtpAddress représente l’adresse de messagerie SMTP correspondant à la boîte aux lettres qui contient le dossier qui sera partagé.
ms.openlocfilehash: 73047dcecfbccb55d74e373891c3154bc7baeeba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464895"
---
# <a name="sendersmtpaddress"></a>SenderSmtpAddress

L’élément **SenderSmtpAddress** représente l’adresse de messagerie SMTP correspondant à la boîte aux lettres qui contient le dossier qui sera partagé. 
  
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
|[GetSharingMetadata](getsharingmetadata.md) <br/> |Définit une demande pour obtenir un jeton d’authentification opaque qui identifie l’invitation de partage.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte qui représente une adresse SMTP est requise.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération de GetSharingMetadata](getsharingmetadata-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

