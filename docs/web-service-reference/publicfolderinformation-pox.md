---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: L’élément PublicFolderInformation contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.
ms.openlocfilehash: bb4432a664024c3d1ccb17826948cfe7a1b58cdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828927"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

L’élément **PublicFolderInformation** contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur. 
  
[Découverte automatique (POX)](autodiscover-pox.md)
  
[Réponse (POX)](response-pox.md)
  
[Compte (POX)](account-pox.md)
  
[PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
```XML
<PublicFolderInformation>
   <SmtpAddress/>
</PublicFolderInformation>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |Contient l’adresse SMTP affectée à la banque de messages de dossier public configurée pour l’utilisateur. Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une requête de découverte automatique pour découvrir les paramètres des dossiers publics.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Compte (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte pour l’utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **PublicFolderInformation** est un élément enfant facultatif de l’élément de **compte** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

