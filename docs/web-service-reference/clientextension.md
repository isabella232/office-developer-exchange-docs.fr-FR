---
title: ClientExtension
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3445ef2b-1bb1-43ea-bc93-85c72401e5b6
description: L’élément ClientExtension contient les informations d’utilisateur et de configuration relatives à une application.
ms.openlocfilehash: d3d9ce1d242a63f28da3464f0faff86abde502c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460196"
---
# <a name="clientextension"></a>ClientExtension

L’élément **ClientExtension** contient les informations d’utilisateur et de configuration relatives à une application. 
  
```XML
<ClientExtension IsAvailable=" true | false " IsMandatory=" true | false " IsEnabledByDefault=" true | false " Type="" Scope="" MarketplaceAssetId="" MarketplaceContentMarket="" AppStatus="" Etoken="">
    <SpecificUsers></SpecificUsers>
    <Manifest></Manifest>
</ClientExtension>
```

 **ClientExtensionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|IsAvailable  <br/> |Indique si l’application est disponible. Une valeur de texte de **true** pour l’attribut **IsAvailable** indique que l’application est disponible. La valeur **false** indique que l’application n’est pas disponible. Cet attribut est facultatif.  <br/> |
|IsMandatory  <br/> |Indique si l’application est obligatoire. Une valeur de texte de **true** pour l’attribut **IsMandatory** indique que l’application est obligatoire pour la boîte aux lettres. La valeur **false** indique que l’application n’est pas obligatoire. Cet attribut est facultatif.  <br/> |
|IsEnabledByDefault  <br/> |Indique si l’application est activée par défaut. Une valeur de texte de **true** pour l’attribut **IsEnabledByDefault** indique que l’application est activée par défaut. La valeur **false** indique que l’application n’est pas activée par défaut. Cet attribut est facultatif.  <br/> |
|ProvidedTo  <br/> |Indique à qui l’application est fournie. Cet attribut est facultatif.  <br/> |
|Type  <br/> |Spécifie le type de l’application.  <br/> |
|Portée  <br/> |Spécifie l’étendue de l’application.  <br/> |
|MarketplaceAssetId  <br/> |Spécifie l’identificateur de l’élément Marketplace de l’application.  <br/> |
|MarketplaceContentMarket  <br/> |Spécifie le contenu Marketplace qu’un utilisateur voit pour obtenir des détails et des avis sur une application.  <br/> |
|AppStatus  <br/> |Spécifie le code d’état d’une application de messagerie dans un état inattendu.  <br/> |
|Etoken  <br/> |Spécifie le jeton de licence pour les applications de messagerie payantes ou d’évaluation.  <br/> |
   
#### <a name="type"></a>Type

|**Valeur**|**Description**|
|:-----|:-----|
|Par défaut  <br/> |Indique que l’application est disponible par défaut.  <br/> |
|Private  <br/> |Indique que l’application est privée.  <br/> |
|Actuel  <br/> |Indique que l’application est une application Marketplace.  <br/> |
   
#### <a name="scope"></a>Portée

|**Valeur**|**Description**|
|:-----|:-----|
|Aucun  <br/> |Indique que l’application n’a pas d’étendue.  <br/> |
|Utilisateur  <br/> |Indique que l’application est par utilisateur.  <br/> |
|Organisation  <br/> |Indique que l’application est destinée à une organisation.  <br/> |
|Par défaut  <br/> |Indique que l’application est une application par défaut.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[SpecificUsers](specificusers.md) <br/> |Spécifie les comptes de messagerie qui peuvent accéder à l’application.  <br/> |
|[Manifeste](manifest.md) <br/> |Contient le fichier manifeste d’application encodé en base 64.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ClientExtensions](clientextensions.md) <br/> |Spécifie un tableau d’éléments **ClientExtension** .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

