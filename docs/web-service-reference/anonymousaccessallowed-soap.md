---
title: AnonymousAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: bf819a65-30f2-4881-a34f-cb30a9c2b6a7
description: L’élément AnonymousAccessAllowed indique si un emplacement de partage de documents nécessite un utilisateur authentifié.
ms.openlocfilehash: b3ff22fbba603bbd74dc08a0dbb1d8687714fe7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466079"
---
# <a name="anonymousaccessallowed-soap"></a>AnonymousAccessAllowed (SOAP)

L’élément **AnonymousAccessAllowed** indique si un emplacement de partage de documents nécessite un utilisateur authentifié. 
  
```XML
<AnonymousAccessAllowed /> 
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Représente les informations d’emplacement et de métadonnées pour un emplacement de partage de documents.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur booléenne de l’élément **AnonymousAccessAllowed** indique si l’emplacement de partage nécessite un utilisateur authentifié. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Éléments XML de découverte automatique SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

