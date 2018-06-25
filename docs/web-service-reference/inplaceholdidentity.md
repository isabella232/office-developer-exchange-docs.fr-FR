---
title: InPlaceHoldIdentity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54f45774-00a0-4392-af1b-8c5f2208a53f
description: L’élément InPlaceHoldIdentity Spécifie l’identité d’une suspension qui conserve les éléments de boîte aux lettres.
ms.openlocfilehash: 954e6ad6c3e0b7786d6bbb8230dba913a32359bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827938"
---
# <a name="inplaceholdidentity"></a>InPlaceHoldIdentity

L’élément **InPlaceHoldIdentity** Spécifie l’identité d’une suspension qui conserve les éléments de boîte aux lettres. 
  
```XML
<InPlaceHoldIdentity></InPlaceHoldIdentity>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[SetHoldOnMailboxes](setholdonmailboxes.md) | [DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **InPlaceHoldIdentity** est l’identificateur de blocage de boîtes aux lettres. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération SetHoldOnMailboxes](setholdonmailboxes-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

