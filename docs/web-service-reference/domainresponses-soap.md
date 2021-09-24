---
title: DomainResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: d9c7fd91-22cd-4c72-a841-25cb9d415e0c
description: L’élément DomainResponses contient un tableau de réponses pour les paramètres de chaque domaine demandé.
ms.openlocfilehash: 307cae0aca0f34b0a33edd41248f8f572f2a80af
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540109"
---
# <a name="domainresponses-soap"></a>DomainResponses (SOAP)

**L’élément DomainResponses contient** un tableau de réponses pour les paramètres de chaque domaine demandé. 
  
```XML
<DomainResponses>
   <DomainResponse/>
</DomainResponses>
```

 **ArrayOfDomainResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contient les paramètres demandés pour le domaine spécifié.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetDomainSettingsResponse (SOAP)](getdomainsettingsresponse-soap.md) <br/> |Représente la réponse à une [demande d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) pour un domaine et renvoie les paramètres de domaine.  <br/> |
|[Response (GetDomainSettings) (SOAP)](response-getdomainsettingssoap.md) <br/> |Représente la réponse à un appel [d’opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md) pour un domaine individuel.  <br/> |
   
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

