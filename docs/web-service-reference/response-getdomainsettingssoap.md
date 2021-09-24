---
title: Response (GetDomainSettings) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: a5b052df-93bd-4fe1-ac30-83de9a3dfcd7
description: L’élément Response représente la réponse à un appel GetDomainSettings pour un domaine individuel.
ms.openlocfilehash: e8f76127d5e812bc6805430544fe334eabd29ffa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540551"
---
# <a name="response-getdomainsettings-soap"></a>Response (GetDomainSettings) (SOAP)

**L’élément Response** représente la réponse à un **appel GetDomainSettings** pour un domaine individuel. 
  
```XML
<Response>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</Response>
```

 **GetDomainSettingsResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Contient la réponse pour chaque domaine demandé dans une **demande GetDomainSettings.**  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Contient le code d’erreur associé à la réponse, le cas échéant.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Contient le message d’erreur associé à la réponse, le cas échéant.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetDomainSettingsResponseMessage (SOAP)](getdomainsettingsresponsemessage-soap.md) <br/> |Renvoie à l’appelant les paramètres de configuration de domaine.  <br/> |
   
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



[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

