---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: L’élément CanModifyPermissions indique si un utilisateur peut modifier les autorisations d’accès à un emplacement de partage de document.
ms.openlocfilehash: 16526cb79eeca591af6e009e67959a1c3b58a5d7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755492"
---
# <a name="canmodifypermissions-soap"></a>CanModifyPermissions (SOAP)

L’élément **CanModifyPermissions** indique si un utilisateur peut modifier les autorisations d’accès à un emplacement de partage de document. 
  
```XML
<CanModifyPermissions /> 
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

La valeur de type Boolean de l’élément **CanModifyPermissions** indique si les utilisateurs peuvent modifier les autorisations d’accès à l’emplacement de partage. 
  
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

