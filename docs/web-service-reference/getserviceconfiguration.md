---
title: GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: acbb29e4-d853-4302-8e32-7018775d54e4
description: L’élément GetServiceConfiguration définit une demande GetServiceConfiguration.
ms.openlocfilehash: fdc4fd84c658dd0cd2ecabe7fefc06113bca173a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59533433"
---
# <a name="getserviceconfiguration"></a>GetServiceConfiguration

**L’élément GetServiceConfiguration** définit une demande GetServiceConfiguration. 
  
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
|[ActingAs](actingas.md) <br/> |Identifie la personne à qui l’appelant envoie l’appel. Cet élément est facultatif. Si cet élément n’est pas présent, l’utilisateur authentifié est supposé être l’expéditeur. **L’élément ActingAs** doit être inclus pour demander des conseils d’expéditeur. Une erreur ErrorInvalidArgument peut être renvoyée dans une réponse si l’élément **ActingAs** est manquant, n’inclut pas de type de routage, n’inclut pas d’adresse de messagerie, contient une adresse de messagerie non valide, n’est pas résolu vers un utilisateur dans les services de domaine Active Directory (AD DS) ou est résolu en plusieurs utilisateurs dans AD DS.  <br/> |
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
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

