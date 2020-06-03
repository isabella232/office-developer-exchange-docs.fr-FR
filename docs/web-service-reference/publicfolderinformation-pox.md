---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: L’élément PublicFolderInformation contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir les informations de dossier public pour l’utilisateur.
ms.openlocfilehash: e044a1feddfaeb4eb93c289c617dde9adc66f332
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457717"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

L’élément **PublicFolderInformation** contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir les informations de dossier public pour l’utilisateur. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |Contient l’adresse SMTP attribuée à la Banque de messages de dossiers publics configurée pour l’utilisateur. Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une demande de découverte automatique pour découvrir les paramètres de dossier public.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Compte (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte de l’utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

L’élément **PublicFolderInformation** est un élément enfant facultatif de l’élément **Account** . 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique de la VARIOle pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

