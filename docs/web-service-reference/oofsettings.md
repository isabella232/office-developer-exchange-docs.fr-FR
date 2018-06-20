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
description: L’élément OofSettings contient les paramètres d’absence du bureau (OOF).
ms.openlocfilehash: d71f068ff24af22da98b6b4de090ab26d3f74f26
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828649"
---
# <a name="oofsettings"></a>OofSettings

L’élément **OofSettings** contient les paramètres d’absence du bureau (OOF). 
  
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

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[OofState](oofstate.md) <br/> |Contient l’état d’absence du bureau de l’utilisateur.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Contient une valeur qui détermine les messages d’absence du bureau externes qui sont envoyés.  <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> |Affiche la durée pour laquelle le statut d’absence du bureau est activé si l’élément [OofState](oofstate.md) est défini sur **planifiées**. Si l’élément [OofState](oofstate.md) est défini sur **activé** ou **désactivé**, la valeur de cet élément est ignorée.  <br/> |
|[InternalReply](internalreply.md) <br/> |Contient la réponse d’absence du bureau envoyée à d’autres utilisateurs dans un domaine ou domaine approuvé de l’utilisateur.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Contient la réponse d’absence du bureau envoyée aux adresses à l’extérieur du destinataire ou les domaines approuvés.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contient les résultats de la réponse et les paramètres d’absence du bureau pour un utilisateur.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserOofSettings](getuseroofsettings-operation.md)
  
[Opération SetUserOofSettings](setuseroofsettings-operation.md)

