---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: L’élément OofSettings contient les paramètres absent (absent (e) du bureau.
ms.openlocfilehash: c1b214fd8bfab5b7a82d41a5187cf6e0fc4ba79c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467192"
---
# <a name="oofsettings"></a>OofSettings

L’élément **OofSettings** contient les paramètres absent (absent (e) du bureau. 
  
[GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
[OofSettings](oofsettings.md)
  
```xml
<OofSettings>
   <OofState>...</OofState>
   <ExternalAudience>...</ExternalAudience>
   <Duration>...</Duration>
   <InternalReply>...</InternalReply>
   <ExternalReply>...</ExternalReply>
</OofSettings>
```

 **UserOofSettings**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |Contient l’état d’absence du Bureau de l’utilisateur.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Contient une valeur qui détermine à qui les messages externes OOF sont envoyés.  <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> |Contient la durée pendant laquelle l’état du Bureau d’absence est activé si l’élément [OofState](oofstate.md) est défini sur **Planifié**. Si l’élément [OofState](oofstate.md) est défini sur **Enabled** ou **Disabled**, la valeur de cet élément est ignorée.  <br/> |
|[InternalReply](internalreply.md) <br/> |Contient la réponse OOF envoyée aux autres utilisateurs du domaine de l’utilisateur ou du domaine approuvé.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Contient la réponse OOF envoyée aux adresses en dehors du domaine du destinataire ou des domaines approuvés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contient les résultats de la réponse et les paramètres OOF d’un utilisateur.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserOofSettings](getuseroofsettings-operation.md)
  
[Opération SetUserOofSettings](setuseroofsettings-operation.md)

