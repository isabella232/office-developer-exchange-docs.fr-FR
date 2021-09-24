---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: L’élément RequestedVersion spécifie la version de service minimale sur qui le client souhaite que la demande soit traitée.
ms.openlocfilehash: 390dee362bf2e6c2bdeac4e0e5564ecbd59b7319
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513331"
---
# <a name="requestedversion-soap"></a>RequestedVersion (SOAP)

**L’élément RequestedVersion** spécifie la version de service minimale sur qui le client souhaite que la demande soit traitée. 
  
```XML
<RequestedVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Request (SOAP)](request-soap.md) <br/> |Contient les paramètres de configuration demandés et les utilisateurs cibles.  <br/> |
|[Request (GetDomainSettings) (SOAP)](request-getdomainsettingssoap.md) <br/> |Représente une demande d’obtenir les paramètres de domaine.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **RequestedVersion** peut être Exchange2010, Exchange2010_SP1, Exchange2010_SP2 ou Exchange2013.
  
## <a name="remarks"></a>Remarques

Si cet élément n’est pas présent, la dernière version du service est utilisée.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

