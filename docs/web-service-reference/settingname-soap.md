---
title: Nom du paramètre (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8bcb0411-58b0-4e37-b97e-00c07dcbecb1
description: L’élément nom du paramètre représente le nom d’un paramètre dans la réponse.
ms.openlocfilehash: 9bf7c8197693bc6887a99ffcbeb2240e1f4c3b20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829468"
---
# <a name="settingname-soap"></a>Nom du paramètre (SOAP)

L’élément **nom du paramètre** représente le nom d’un paramètre dans la réponse. 
  
```XML
<SettingName/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UserSettingError (SOAP)](usersettingerror-soap.md) <br/> |Représente une erreur est renvoyée lors de la récupération d’un paramètre de l’utilisateur.  <br/> |
|[DomainSettingError (SOAP)](domainsettingerror-soap.md) <br/> |Représente une erreur s’est produite lors de la récupération d’un paramètre du domaine. Cela représente une erreur à partir d’une demande **GetDomainSettings** .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de l’élément du **nom du paramètre** représente le nom d’un paramètre dans une réponse. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   

