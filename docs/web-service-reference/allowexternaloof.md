---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: L’élément AllowExternalOof contient une valeur qui identifie auquel sont envoyés les messages d’absence du bureau (OOF) externes.
ms.openlocfilehash: 1c87a51676bf6e44b2e650a4e973d0ab89a52e31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755200"
---
# <a name="allowexternaloof"></a>AllowExternalOof

L’élément **AllowExternalOof** contient une valeur qui identifie auquel sont envoyés les messages d’absence du bureau (OOF) externes. 
  
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
- [AllowExternalOof](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contient les résultats de la réponse et les paramètres d’absence du bureau pour un utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte est nécessaire pour cet élément. Le tableau suivant répertorie les valeurs possibles de cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|**None** <br/> |Expéditeurs en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur ne recevra pas une réponse de message d’absence du bureau externe.  <br/> |
|**Connus** <br/> |Expéditeurs en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur seulement reçoit une réponse de message d’absence du bureau externe si l’expéditeur se trouve dans Exchange l’utilisateur stockent la liste des contacts.  <br/> |
|**All** <br/> |Expéditeurs en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur reçoit une réponse de message d’absence du bureau externe.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément partageant le même type que l’élément [ExternalAudience](externalaudience.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserOofSettings](getuseroofsettings-operation.md) 
- [Opération SetUserOofSettings](setuseroofsettings-operation.md)

