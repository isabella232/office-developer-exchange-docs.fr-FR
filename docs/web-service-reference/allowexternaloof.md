---
title: AllowExternalOof
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AllowExternalOof
api_type:
- schema
ms.assetid: e5387172-5b92-4bb1-8394-180e9c7ff771
description: L’élément AllowExternalOof contient une valeur qui identifie à qui les messages externes hors Office (OOF) sont envoyés.
ms.openlocfilehash: 7d2e34797af8a9e9d11570a5ea2e618db7630f0c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523223"
---
# <a name="allowexternaloof"></a>AllowExternalOof

**L’élément AllowExternalOof** contient une valeur qui identifie à qui les messages externes hors Office (OOF) sont envoyés. 
  
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
|[GetUserOofSettingsResponse](getuseroofsettingsresponse.md) <br/> |Contient les résultats de la réponse et les paramètres d’absence du travail d’un utilisateur.  <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise pour cet élément. Le tableau suivant répertorie les valeurs possibles pour cet élément.
  
|**Valeur**|**Description**|
|:-----|:-----|
|**Aucun** <br/> |Les expéditeurs de messages électroniques en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur ne reçoivent pas de réponse externe au message d’absence du service.  <br/> |
|**Known** <br/> |Les expéditeurs de messages électroniques en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur ne reçoivent une réponse de message d’absence du travail externe que si l’expéditeur se trouve dans la liste de contacts du magasin Exchange de l’utilisateur.  <br/> |
|**All** <br/> |Les expéditeurs de messages électroniques en dehors de l’organisation de l’utilisateur de boîte aux lettres qui envoient des messages à l’utilisateur reçoivent une réponse externe au message d’absence du service.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément partage le même type que [l’élément ExternalAudience.](externalaudience.md) 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserOofSettings](getuseroofsettings-operation.md) 
- [Opération SetUserOofSettings](setuseroofsettings-operation.md)

