---
title: DomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f3d37f5a-c9ea-4ed9-a011-94d33bda64d1
description: L’élément DomainSettings représente les paramètres de domaine qui ont été envoyés dans une demande de découverte automatique ou renvoyés par une réponse de découverte automatique.
ms.openlocfilehash: 67e3753b0cf5c7c653664ff087f697ce7ae2b7a4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530697"
---
# <a name="domainsettings-soap"></a>DomainSettings (SOAP)

L’élément **DomainSettings** représente les paramètres de domaine qui ont été envoyés dans une demande de découverte automatique ou renvoyés par une réponse de découverte automatique. 
  
```XML
<DomainSettings>
   <DomainSetting/>
</DomainSettings>
```

 **DomainSettings**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DomainSetting (SOAP)](domainsetting-soap.md) <br/> |Contient les paramètres de domaine qui sont renvoyés par une demande [SOAP (GetDomainSettings Operation)](getdomainsettings-operation-soap.md) .  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contient les paramètres demandés pour le domaine spécifié.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

