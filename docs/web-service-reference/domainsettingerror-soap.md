---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: L’élément DomainSettingError représente une erreur qui s’est produite lors de la récupération d’un paramètre de domaine. Il s’agit d’une erreur provenant d’une demande GetDomainSettings.
ms.openlocfilehash: d2d7e1fc1509ade88de0013cb9e4ff54712d0f56
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530146"
---
# <a name="domainsettingerror-soap"></a>DomainSettingError (SOAP)

**L’élément DomainSettingError** représente une erreur qui s’est produite lors de la récupération d’un paramètre de domaine. Il s’agit d’une erreur provenant **d’une demande GetDomainSettings.** 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 **DomainSettingError**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Identifie le code d’erreur associé à la demande spécifique.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Contient le message d’erreur associé à la demande spécifique.  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |Représente le nom du paramètre.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Contient des informations d’erreur pour les paramètres qui n’ont pas pu être renvoyés.  <br/> |
   
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

