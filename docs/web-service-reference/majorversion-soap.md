---
title: MajorVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0b2a83cf-e173-4073-9603-b2ea3b36ec1a
description: L’élément MajorVersion représente le numéro de version principale du serveur.
ms.openlocfilehash: 2c564b110ec7497a2e9c92a00bfb7f376a657849
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44531006"
---
# <a name="majorversion-soap"></a>MajorVersion (SOAP)

L’élément **MajorVersion** représente le numéro de version principale du serveur. 
  
```XML
<MajorVersion/>
```

 **int**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ServerVersionInfo (SOAP)](serverversioninfo-soap.md) <br/> |Contient la version du serveur qui a traité la demande.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **MajorVersion** est un entier qui représente le numéro de version principale du serveur qui a traité la demande. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

