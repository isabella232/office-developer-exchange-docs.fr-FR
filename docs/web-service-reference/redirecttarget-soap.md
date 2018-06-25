---
title: RedirectTarget (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f8162724-cf9a-4543-a1ad-5846c8b10bfa
description: L’élément RedirectTarget (SOAP) contient la cible de la redirection URL ou adresse de messagerie.
ms.openlocfilehash: 3a8a0c39c6889730c9d17778c6a26f84fcbcd4a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829019"
---
# <a name="redirecttarget-soap"></a>RedirectTarget (SOAP)

L’élément [RedirectTarget (SOAP)](redirecttarget-soap.md) contient la cible de la redirection URL ou adresse de messagerie. 
  
```XML
<RedirectTarget/>
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
|[Réponse de l’utilisateur (SOAP)](userresponse-soap.md) <br/> |Représente une réponse à une demande de GetUserSettings pour un utilisateur individuel.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contient les paramètres requis pour le domaine spécifié.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

La valeur de texte contient la cible de la redirection URL ou l’adresse électronique qui doit être utilisé pour un GetUserSettings ultérieures ou demander des GetDomainSettings.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   

