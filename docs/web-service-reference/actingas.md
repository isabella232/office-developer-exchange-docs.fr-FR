---
title: ActingAs
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
description: L’élément ActingAs identifie qui envoie en tant que l’appelant.
ms.openlocfilehash: 9c007ed45f85dba265261dd79a6fd846dbd9d2f9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756336"
---
# <a name="actingas"></a>ActingAs

L’élément **ActingAs** identifie qui envoie en tant que l’appelant. 
  
```xml
<ActingAs>
   <EmailAddress/>
   <RoutingType/>
</ActingAs>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) <br/> |Définit l’adresse SMTP Simple Mail Transfer Protocol () d’un utilisateur de boîte aux lettres. Cet élément est facultatif.  <br/> |
|[RoutingType (EmailAddress)](routingtype-emailaddress.md) <br/> |Définit le routage est utilisé pour la boîte aux lettres. La valeur par défaut est SMTP. Cet élément est facultatif.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetServiceConfiguration](getserviceconfiguration.md) <br/> |Définit une demande **GetServiceConfiguration** .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est facultatif. Si cet élément n’est pas présent, l’utilisateur authentifié est supposé être l’expéditeur. L’élément **ActingAs** doit être inclus pour demander des conseils de l’expéditeur. Une erreur **ErrorInvalidArgument** peut être renvoyée dans une réponse si l’élément **ActingAs** est manquant, n’inclut pas un type de routage, n’inclut pas une adresse de messagerie, contient une adresse de messagerie non valides, ne correspond pas à un utilisateur dans Active Directory Domaine Services (AD DS), ou correspond à plusieurs utilisateurs dans AD DS. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

