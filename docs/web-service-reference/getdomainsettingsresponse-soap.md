---
title: GetDomainSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43ebd17b-3a70-4878-9254-97a4c2c87b77
description: L’élément GetDomainSettingsResponse représente la réponse à une opération GetDomainSettings (SOAP), qui retourne les paramètres de domaine.
ms.openlocfilehash: c4984c2c6c532fcbd45c1a75733e578f6d9491fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756584"
---
# <a name="getdomainsettingsresponse-soap"></a>GetDomainSettingsResponse (SOAP)

L’élément **GetDomainSettingsResponse** représente la réponse à une [opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md), qui retourne les paramètres de domaine.
  
```XML
<GetDomainSettingsResponse>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</GetDomainSettingsResponse>
```

 **GetDomainSettingsResponse**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DomainResponses (SOAP)](domainresponses-soap.md) <br/> |Contient un tableau de réponses pour les paramètres de chaque domaine demandé.  <br/> |
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Représente un code d’erreur retourné par le service de découverte automatique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Représente un message qui est associé à un code d’erreur retourné par le service de découverte automatique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

