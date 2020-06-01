---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: L’élément GetServiceConfiguration définit une demande GetServiceConfiguration.
ms.openlocfilehash: e9357a9e3be22e129c4910c01231f9dbd22a2dbe
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457871"
---
# <a name="getserviceconfiguration"></a>GetServiceConfiguration

L’élément **GetServiceConfiguration** définit une demande GetServiceConfiguration. 
  
```XML
<GetServiceConfiguration>
   <ActingAs/>
   <RequestedConfiguration/>
</GetServiceConfiguration>
```

 **GetServiceConfigurationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Actionas](actingas.md) <br/> |Identifie les personnes qui envoient l’appelant. Cet élément est facultatif. Si cet élément n’est pas présent, l’utilisateur authentifié est supposé être l’expéditeur. L’élément **actionas** doit être inclus pour la demande d’indications de l’expéditeur. Une erreur ErrorInvalidArgument peut être renvoyée dans une réponse si l’élément **actionas** est manquant, qu’il n’inclut pas de type de routage, qu’il n’inclut pas d’adresse de messagerie, qu’il contient une adresse de messagerie non valide, qu’il n’est pas résolu en utilisateur dans les services de domaine Active Directory (AD DS) ou qu’il est résolu en plusieurs utilisateurs dans AD DS.  <br/> |
|[RequestedConfiguration](requestedconfiguration.md) <br/> |Contient les configurations de service demandées. Cet élément est obligatoire.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

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

