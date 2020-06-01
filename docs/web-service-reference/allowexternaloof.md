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
description: L’élément AllowExternalOof contient une valeur qui identifie l’expéditeur des messages d’absence du Bureau externes.
ms.openlocfilehash: e4934bc4bc86e1f9f764279a13ecaeca073d9e5d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464811"
---
# <a name="allowexternaloof"></a>AllowExternalOof

L’élément **AllowExternalOof** contient une valeur qui identifie l’expéditeur des messages d’absence du Bureau externes. 
  
- [GetUserOofSettingsResponse](getuseroofsettingsresponse.md)
  
- [AllowExternalOof](allowexternaloof.md)
  
```xml
<AllowExternalOof>None or Known or All</AllowExternalOof>
```

 **ExternalAudience**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contient les résultats de la réponse et les paramètres OOF d’un utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise pour cet élément. Le tableau suivant répertorie les valeurs possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|**Aucun** <br/> |Les expéditeurs de messages électroniques situés en dehors de l’organisation de l’utilisateur de la boîte aux lettres qui envoient des messages à l’utilisateur ne reçoivent pas de réponse externe aux messages OOF.  <br/> |
|**Connus** <br/> |Les expéditeurs de messages électroniques extérieurs à l’organisation de l’utilisateur de la boîte aux lettres qui envoie des messages à l’utilisateur recevront uniquement une réponse externe aux messages OOF si l’expéditeur se trouve dans la liste des contacts de la banque Exchange de l’utilisateur.  <br/> |
|**All** <br/> |Les expéditeurs de messages électroniques extérieurs à l’organisation de l’utilisateur de la boîte aux lettres qui envoie des messages à l’utilisateur recevront une réponse externe aux messages OOF.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément partage le même type que l’élément [ExternalAudience](externalaudience.md) . 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserOofSettings](getuseroofsettings-operation.md) 
- [Opération SetUserOofSettings](setuseroofsettings-operation.md)

