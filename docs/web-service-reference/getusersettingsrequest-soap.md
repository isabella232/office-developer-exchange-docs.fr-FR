---
title: GetUserSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: L’élément GetUserSettingsRequest représente une demande de récupération des paramètres spécifiés pour un ou plusieurs utilisateurs.
ms.openlocfilehash: ccbcd67d4fdcb98be08acfecbf2ae066a91d65d2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547392"
---
# <a name="getusersettingsrequest-soap"></a>GetUserSettingsRequest (SOAP)

**L’élément GetUserSettingsRequest** représente une demande de récupération des paramètres spécifiés pour un ou plusieurs utilisateurs. 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
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

Aucun.
  
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

