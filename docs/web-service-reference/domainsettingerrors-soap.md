---
title: DomainSettingErrors (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a4ce19de-f560-4984-8047-ecbbc86c9b91
description: L’élément DomainSettingsErrors contient des informations d’erreur pour les paramètres qui n’ont pas pu être renvoyés.
ms.openlocfilehash: 4e7ee29c2bc680a1938b75189c2ac3c214f7d2b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530704"
---
# <a name="domainsettingerrors-soap"></a>DomainSettingErrors (SOAP)

L’élément **DomainSettingsErrors** contient des informations d’erreur pour les paramètres qui n’ont pas pu être renvoyés. 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 **DomainSettingsErrors**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DomainSettingError (SOAP)](domainsettingerror-soap.md) <br/> |Représente une erreur qui s’est produite lors de la récupération d’un paramètre de domaine. Cela représente une erreur à partir d’une demande d’opération [SOAP (GetDomainSettings Operation)](getdomainsettings-operation-soap.md) .  <br/> |
   
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

