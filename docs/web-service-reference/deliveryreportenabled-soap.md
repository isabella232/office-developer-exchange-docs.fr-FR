---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: L’élément DeliveryReportEnabled représente l’indicateur DeliveryReportEnabled(). L’élément DeliveryReportEnabled est uniquement à usage interne. Cet élément n’est pas utilisé par les clients.
ms.openlocfilehash: 95fe62e25ca871171b398b17f3d03dff9235001b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510168"
---
# <a name="deliveryreportenabled-soap"></a>DeliveryReportEnabled (SOAP)

**L’élément DeliveryReportEnabled représente** **l’indicateur DeliveryReportEnabled().** **L’élément DeliveryReportEnabled est** uniquement à usage interne. Cet élément n’est pas utilisé par les clients. 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
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

Une valeur de texte true pour l’élément DeliveryReportEnabled indique que les rapports de remise des utilisateurs de l’organisation peuvent être utilisés. La valeur false indique que les rapports de remise doivent être supprimés.
  
## <a name="remarks"></a>Remarques

Utilisez cet élément pour autoriser ou supprimer des rapports de remise à partir du serveur.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

