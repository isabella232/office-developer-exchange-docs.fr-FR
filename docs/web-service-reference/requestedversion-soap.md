---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: L’élément RequestedVersion spécifie la version minimale de service que le client souhaite le traitement sur la demande.
ms.openlocfilehash: 0d8682c33790d2d26001512ad9e2191ae52074d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829134"
---
# <a name="requestedversion-soap"></a>RequestedVersion (SOAP)

L’élément **RequestedVersion** spécifie la version minimale de service que le client souhaite le traitement sur la demande. 
  
```XML
<RequestedVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Demande (SOAP)](request-soap.md) <br/> |Contient les paramètres de configuration requise et les utilisateurs cibles.  <br/> |
|[Demande (GetDomainSettings) (SOAP)](request-getdomainsettingssoap.md) <br/> |Représente une demande pour obtenir les paramètres de domaine.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte pour l’élément **RequestedVersion** peut être Exchange2010, Exchange2010_SP1, Exchange2010_SP2 ou Exchange2013.
  
## <a name="remarks"></a>Remarques

Si cet élément n’est pas présent, la dernière version de service est utilisée.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

