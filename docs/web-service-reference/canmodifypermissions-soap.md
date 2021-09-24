---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: L’élément CanModifyPermissions indique si un utilisateur peut modifier les autorisations d’accès à un emplacement de partage de documents.
ms.openlocfilehash: 5aa11ff62fc5c82d263eb03707d7514b87c94be0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515984"
---
# <a name="canmodifypermissions-soap"></a>CanModifyPermissions (SOAP)

**L’élément CanModifyPermissions indique** si un utilisateur peut modifier les autorisations d’accès à un emplacement de partage de documents. 
  
```XML
<CanModifyPermissions /> 
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

La valeur booléle de **l’élément CanModifyPermissions** indique si les utilisateurs peuvent modifier les autorisations d’accès à l’emplacement de partage. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Référence de service web de découverte automatique pour Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Éléments XML de découverte automatique SOAP pour Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

