---
title: Request (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 75696436-997e-49f1-a31b-eb9a8c3526f3
description: L’élément Request contient les paramètres de configuration demandés et les utilisateurs cibles.
ms.openlocfilehash: 533419d6e622bb1d415f739868aaf30c79c41635
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542804"
---
# <a name="request-soap"></a>Request (SOAP)

**L’élément Request** contient les paramètres de configuration demandés et les utilisateurs cibles. 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 **GetUserSettingsRequest**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Users (SOAP)](users-soap.md) <br/> |Représente une collection d’adresses de messagerie des utilisateurs pour lesquels les paramètres doivent être récupérés.  <br/> |
|[RequestedSettings (SOAP)](requestedsettings-soap.md) <br/> |Contient les noms des paramètres de configuration demandés.  <br/> |
|[RequestedVersion (SOAP)](requestedversion-soap.md) <br/> |Spécifie la version du serveur spécifique que le fournisseur souhaite utiliser.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserSettingsRequestMessage (SOAP)](getusersettingsrequestmessage-soap.md) <br/> |Représente une [demande d’opération GetUserSettings (SOAP).](getusersettings-operation-soap.md)  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucune.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Nom du schéma  <br/> |Schéma de découverte automatique  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |True  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserSettings (SOAP)](getusersettings-operation-soap.md)

