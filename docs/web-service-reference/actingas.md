---
title: Actionas
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ActingAs
api_type:
- schema
ms.assetid: 3896afff-5c2c-4eaf-8621-c70e0371ea78
description: L’élément Actionas identifie les personnes qui envoient l’appelant.
ms.openlocfilehash: 175a03018ee3529ec595dbe9afb7dc61ad6afc35
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529699"
---
# <a name="actingas"></a>Actionas

L’élément **actionas** identifie les personnes qui envoient l’appelant. 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Définit l’adresse SMTP (Simple Mail Transfer Protocol) d’un utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Définit le routage utilisé pour la boîte aux lettres. La valeur par défaut est SMTP. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetServiceConfiguration](getserviceconfiguration.md) <br/> |Définit une requête **GetServiceConfiguration** .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est facultatif. Si cet élément n’est pas présent, l’utilisateur authentifié est supposé être l’expéditeur. L’élément **actionas** doit être inclus pour la demande d’indications de l’expéditeur. Une erreur **ErrorInvalidArgument** peut être renvoyée dans une réponse si l’élément **actionas** est manquant, qu’il n’inclut pas de type de routage, qu’il n’inclut pas d’adresse de messagerie, qu’il contient une adresse de messagerie non valide, qu’il n’est pas résolu en utilisateur dans les services de domaine Active Directory (AD DS) ou qu’il est résolu en plusieurs utilisateurs dans AD DS. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

