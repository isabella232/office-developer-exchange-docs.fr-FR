---
title: GetDomainSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: L’élément GetDomainSettingsRequest représente une demande d’opération SOAP (GetDomainSettings Operation).
ms.openlocfilehash: 400016d0817131fb70ec7ff3db7fbfdc1b51f8f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460959"
---
# <a name="getdomainsettingsrequest-soap"></a>GetDomainSettingsRequest (SOAP)

L’élément **GetDomainSettingsRequest** représente une demande d’opération [SOAP (GetDomainSettings Operation)](getdomainsettings-operation-soap.md) . 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 **GetDomainSettingsRequest**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Domaines (SOAP)](domains-soap.md) <br/> |Représente une collection d’identificateurs de domaine.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contient les noms des paramètres de configuration de domaine demandés.  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |Spécifie la version du serveur que le fournisseur doit utiliser.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
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



[Opération GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

