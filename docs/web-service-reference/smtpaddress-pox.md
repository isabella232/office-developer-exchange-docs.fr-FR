---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: L’élément SmtpAddress contient l’adresse SMTP attribuée à la magasin de messages de dossier public configurée pour l’utilisateur.
ms.openlocfilehash: d257b193a3254afceaa72d396a8c2724bb3165c6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546986"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

**L’élément SmtpAddress** contient l’adresse SMTP attribuée à la magasin de messages de dossier public configurée pour l’utilisateur. 
  
- [AutoDiscover (POX)](autodiscover-pox.md)
  
- [Response (POX)](response-pox.md)
  
- [Account (POX)](account-pox.md)
  
- [PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
- [SmtpAddress (POX)](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique afin de découvrir des informations de dossier public pour l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte représente l’adresse SMTP affectée à la magasin de dossiers publics configurée pour l’utilisateur. Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une demande de découverte automatique pour découvrir les paramètres de dossier public. 
  
## <a name="remarks"></a>Remarques

**L’élément SmtpAddress** est un élément enfant requis de l’élément **PublicFolderInformation.** 
  
## <a name="see-also"></a>Voir aussi

- [Éléments XML de découverte automatique POX pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

