---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: L’élément FreeBusyAccessEnabled représente l’indicateur FreeBusyAccessEnabled(). L’élément FreeBusyAccessEnabled est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: faf51798ba211b4219a3f2abee3b3e5e9ce4ab29
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530214"
---
# <a name="freebusyaccessenabled-soap"></a>FreeBusyAccessEnabled (SOAP)

**L’élément FreeBusyAccessEnabled** représente l’indicateur **FreeBusyAccessEnabled().** **L’élément FreeBusyAccessEnabled** est à usage interne uniquement. Cet élément n’est pas utilisé par les clients. 
  
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
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Représente une liste de relations organisationnelles pour une seule organisation.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte **true** pour l’élément **FreeBusyAccessEnabled** indique que la relation de partage doit être utilisée pour récupérer des informations de libre-service auprès des utilisateurs de l’organisation. La valeur **false** indique que la relation de partage doit être supprimée. 
  
## <a name="remarks"></a>Remarques

Utilisez cet élément pour autoriser ou supprimer les informations de libre/occupé du serveur. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

