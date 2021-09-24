---
title: PublicFolderInformation (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6
description: L’élément PublicFolderInformation contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir des informations de dossier public pour l’utilisateur.
ms.openlocfilehash: d77ea350f05c5d6137d3b67cfd49119bf9590e53
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540621"
---
# <a name="publicfolderinformation-pox"></a>PublicFolderInformation (POX)

**L’élément PublicFolderInformation** contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir des informations de dossier public pour l’utilisateur. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
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
|[SmtpAddress (POX)](smtpaddress-pox.md) <br/> |Contient l’adresse SMTP attribuée à la magasin de messages de dossiers publics configurée pour l’utilisateur. Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une demande de découverte automatique pour découvrir les paramètres de dossier public.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |Spécifie les paramètres de compte de l’utilisateur.  <br/> |
   
## <a name="remarks"></a>Remarques

**L’élément PublicFolderInformation** est un élément enfant facultatif de **l’élément Account.** 
  
## <a name="see-also"></a>Voir aussi



[Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

