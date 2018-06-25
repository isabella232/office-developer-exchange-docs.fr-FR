---
title: Demande (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75696436-997e-49f1-a31b-eb9a8c3526f3
description: L’élément de demande contient les paramètres de configuration requise et les utilisateurs cibles.
ms.openlocfilehash: dfea33786066dd7803d0fd061cbb87bb06d11531
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829125"
---
# <a name="request-soap"></a>Demande (SOAP)

L’élément **demande** contient les paramètres de configuration requise et les utilisateurs cibles. 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 **GetUserSettingsRequest**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Utilisateurs (SOAP)](users-soap.md) <br/> |Représente une collection d’adresses de messagerie des utilisateurs pour lesquels les paramètres doivent être récupérés.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contient les noms des paramètres de configuration demandé.  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |Spécifie la version de serveur spécifique que le fournisseur souhaite utiliser.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserSettingsRequestMessage (SOAP)](getusersettingsrequestmessage-soap.md) <br/> |Représente une demande [d’opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) .  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)

