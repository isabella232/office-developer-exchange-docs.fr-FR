---
title: RequestedSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8d713d22-580c-49a5-99f5-ee532443e89a
description: L’élément RequestedSettings contient les noms des paramètres de configuration demandés.
ms.openlocfilehash: e94c02d8f92d7aaac619c58f093c536cc1a098bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465295"
---
# <a name="requestedsettings-soap"></a>RequestedSettings (SOAP)

L’élément **RequestedSettings** contient les noms des paramètres de configuration demandés. 
  
```XML
<RequestedSettings>
   <Setting/>
</RequestedSettings>
```

 **RequestedSettings**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Paramètre (SOAP)](setting-soap.md) <br/> |Représente un paramètre de configuration à renvoyer.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserSettingsRequest (SOAP)](getusersettingsrequest-soap.md) <br/> |Représente une demande de récupération des paramètres spécifiés pour un ou plusieurs utilisateurs.  <br/> |
|[Demande (SOAP)](request-soap.md) <br/> |Contient les paramètres de configuration demandés et les utilisateurs cibles.  <br/> |
|[GetDomainSettingsRequest (SOAP)](getdomainsettingsrequest-soap.md) <br/> |Représente une demande d' [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
   
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

