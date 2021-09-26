---
title: DomainSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: bad5399c-0762-4979-9c15-58cf4b7b6278
description: L’élément DomainSetting contient les paramètres de domaine renvoyés par la demande d’opération SOAP (GetDomainSettings operation).
ms.openlocfilehash: 19c88e6f3f517d012a5c51f548da3d3776770444
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541447"
---
# <a name="domainsetting-soap"></a>DomainSetting (SOAP)

**L’élément DomainSetting** contient les paramètres de domaine renvoyés par la demande d’opération [SOAP (GetDomainSettings](getdomainsettings-operation-soap.md) operation). 
  
```XML
<DomainSetting>
   <Name/>
</DomainSetting>
```

 **DomainSetting**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Name (SOAP)](name-soap.md) <br/> |Représente le nom d’un paramètre.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DomainSettings (SOAP)](domainsettings-soap.md) <br/> |Représente les paramètres de domaine qui ont été envoyés dans une demande de découverte automatique ou renvoyés par une réponse de découverte automatique.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

