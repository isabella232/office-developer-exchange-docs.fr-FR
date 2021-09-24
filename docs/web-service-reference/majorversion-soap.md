---
title: MajorVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 0b2a83cf-e173-4073-9603-b2ea3b36ec1a
description: L’élément MajorVersion représente le numéro de version principal du serveur.
ms.openlocfilehash: eb6bed958e36cbd3c0c35825ff10d857ea839cff
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511095"
---
# <a name="majorversion-soap"></a>MajorVersion (SOAP)

**L’élément MajorVersion** représente le numéro de version principal du serveur. 
  
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
|[ServerVersionInfo (SOAP)](serverversioninfo-soap.md) <br/> |Contient la version du serveur qui a traitée la demande.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **MajorVersion** est un nombre intégral qui représente le numéro de version principal du serveur qui a traitée la demande. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Opération GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)

