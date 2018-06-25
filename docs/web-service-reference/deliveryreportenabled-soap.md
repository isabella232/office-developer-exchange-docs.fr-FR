---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: L’élément DeliveryReportEnabled représente l’indicateur DeliveryReportEnabled(). L’élément DeliveryReportEnabled est à usage interne uniquement. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 089256a5f75ad92a4f11c5aaf3d175382eeee456
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755891"
---
# <a name="deliveryreportenabled-soap"></a>DeliveryReportEnabled (SOAP)

L’élément **DeliveryReportEnabled** représente l’indicateur **DeliveryReportEnabled()** . L’élément **DeliveryReportEnabled** est à usage interne uniquement. Cet élément n’est pas utilisé par les clients. 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
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
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Représente une liste des relations d’organisation pour une organisation unique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte de la valeur true pour l’élément DeliveryReportEnabled indique que vous pouvant utiliser les rapports de remise parmi les utilisateurs de l’organisation. La valeur false indique que les rapports de remise doit être supprimée.
  
## <a name="remarks"></a>Remarques

Utilisez cet élément pour autoriser ou supprimer des rapports de remise à partir du serveur.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

