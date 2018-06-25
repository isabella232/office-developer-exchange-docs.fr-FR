---
title: ExternalAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 967df8c0-ee95-4202-b037-0c4b9fbbf5ee
description: L’élément ExternalAccessAllowed indique si un emplacement de partage de documents sont disponible à l’extérieur des connexions.
ms.openlocfilehash: 7d2a4027fe6de0c24191272d65605310af6a16bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756318"
---
# <a name="externalaccessallowed-soap"></a>ExternalAccessAllowed (SOAP)

L’élément **ExternalAccessAllowed** indique si un emplacement de partage de documents sont disponible à l’extérieur des connexions. 
  
```XML
<ExternalAccessAllowed /> 
```

 **Boolean**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Représente les informations d’emplacement et les métadonnées pour un emplacement de partage de document.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de type Boolean de l’élément **ExternalAccessAllowed** indique si l’emplacement de partage est disponible pour les connexions à l’extérieur de. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Éléments du fichier XML Autodiscover SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

