---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: L’élément FreeBusyAccessEnabled représente l’indicateur FreeBusyAccessEnabled (). L’élément FreeBusyAccessEnabled est réservé à un usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: c148d8fa1301339f8579884dc02b6c9e452f3035
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461295"
---
# <a name="freebusyaccessenabled-soap"></a>FreeBusyAccessEnabled (SOAP)

L’élément **FreeBusyAccessEnabled** représente l’indicateur **FreeBusyAccessEnabled ()** . L’élément **FreeBusyAccessEnabled** est réservé à un usage interne. Cet élément n’est pas utilisé par les clients. 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
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
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Représente une liste de relations d’organisation pour une seule organisation.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte de **true** pour l’élément **FreeBusyAccessEnabled** indique que la relation de partage doit être utilisée pour récupérer les informations de disponibilité des utilisateurs de l’organisation. La valeur **false** indique que la relation de partage doit être supprimée. 
  
## <a name="remarks"></a>Remarques

Utilisez cet élément pour autoriser ou supprimer les informations de disponibilité du serveur. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

