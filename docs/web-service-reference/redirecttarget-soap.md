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
description: L’élément RedirectTarget (SOAP) contient la cible de l’URL de redirection ou de l’adresse de messagerie.
ms.openlocfilehash: 092d575560379d43b12dd98a3efa155b59c31450
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462198"
---
# <a name="redirecttarget-soap"></a>RedirectTarget (SOAP)

L’élément [RedirectTarget (SOAP)](redirecttarget-soap.md) contient la cible de l’URL de redirection ou de l’adresse de messagerie. 
  
```XML
<RedirectTarget/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UserResponse (SOAP)](userresponse-soap.md) <br/> |Représente une réponse à une demande GetUserSettings pour un utilisateur individuel.  <br/> |
|[DomainResponse (SOAP)](domainresponse-soap.md) <br/> |Contient les paramètres demandés pour le domaine spécifié.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur texte contient la cible de l’URL de redirection ou de l’adresse de messagerie à utiliser pour une requête GetUserSettings ou GetDomainSettings ultérieure.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |messages. xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   

