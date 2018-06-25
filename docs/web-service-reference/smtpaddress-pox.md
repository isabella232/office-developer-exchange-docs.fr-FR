---
title: SmtpAddress (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 984ccd97-c337-47b6-ba42-3405a8b55a71
description: L’élément SmtpAddress contient l’adresse SMTP affectée à la banque de messages de dossier public configurée pour l’utilisateur.
ms.openlocfilehash: 43ebb328e31cdec11412e80b743d4d4393b7960a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829507"
---
# <a name="smtpaddress-pox"></a>SmtpAddress (POX)

L’élément **SmtpAddress** contient l’adresse SMTP affectée à la banque de messages de dossier public configurée pour l’utilisateur. 
  
- [Découverte automatique (POX)](autodiscover-pox.md)
  
- [Réponse (POX)](response-pox.md)
  
- [Compte (POX)](account-pox.md)
  
- [PublicFolderInformation (POX)](publicfolderinformation-pox.md)
  
- [SmtpAddress (POX)](smtpaddress-pox.md)
  
```XML
<SmtpAddress/>
```

## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[PublicFolderInformation (POX)](publicfolderinformation-pox.md) <br/> |Contient des informations que les clients peuvent utiliser pour envoyer une demande de découverte automatique pour découvrir les informations de dossier public pour l’utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de text représente l’adresse SMTP affectée à la banque de dossiers publics configurée pour l’utilisateur. Cette adresse SMTP peut être utilisée dans l’élément [EMailAddress (POX)](emailaddress-pox.md) d’une requête de découverte automatique pour découvrir les paramètres des dossiers publics. 
  
## <a name="remarks"></a>Remarques

L’élément **SmtpAddress** est un élément enfant requis de l’élément **PublicFolderInformation** . 
  
## <a name="see-also"></a>Voir aussi

- [Éléments du fichier XML Autodiscover variole pour Exchange](pox-autodiscover-xml-elements-for-exchange.md)

