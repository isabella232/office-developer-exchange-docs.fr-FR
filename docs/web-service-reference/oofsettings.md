---
title: OofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- OofSettings
api_type:
- schema
ms.assetid: 8f37d174-db11-427c-bbed-fdde754a60c7
description: L’élément OofSettings contient les paramètres De Office (OOF).
ms.openlocfilehash: 0a612cacb69464dfda3c1f235c32f569d3e45775
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543169"
---
# <a name="oofsettings"></a>OofSettings

**L’élément OofSettings** contient les paramètres De Office (OOF). 
  
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
|[OofState](oofstate.md) <br/> |Contient l’état d’absence du travail de l’utilisateur.  <br/> |
|[ExternalAudience](externalaudience.md) <br/> |Contient une valeur qui détermine à qui les messages d’absence du système externes sont envoyés.  <br/> |
|[Durée (UserOofSettings)](duration-useroofsettings.md) <br/> |Contient la durée pendant laquelle l’état d’absence du travail est activé si l’élément [OofState](oofstate.md) est définie sur **Scheduled**. Si [l’élément OofState](oofstate.md) est activé ou **désactivé,** la valeur de cet élément est ignorée.   <br/> |
|[InternalReply](internalreply.md) <br/> |Contient la réponse OOF envoyée à d’autres utilisateurs dans le domaine ou le domaine approuvé de l’utilisateur.  <br/> |
|[ExternalReply](externalreply.md) <br/> |Contient la réponse OOF envoyée aux adresses en dehors du domaine du destinataire ou des domaines de confiance.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contient les résultats de la réponse et les paramètres d’absence du travail d’un utilisateur.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserOofSettings](getuseroofsettings-operation.md)
  
[Opération SetUserOofSettings](setuseroofsettings-operation.md)

