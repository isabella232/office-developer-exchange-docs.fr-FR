---
title: FreeBusyResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FreeBusyResponse
api_type:
- schema
ms.assetid: 3038d106-9ac9-4ac7-bb43-96c783edbef5
description: L’élément FreeBusyResponse contient les informations de libre/occupé d’un utilisateur de boîte aux lettres unique.
ms.openlocfilehash: 7be7eb7a5ae72be8c9da916fb861d9cce686bc34
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511581"
---
# <a name="freebusyresponse"></a>FreeBusyResponse

**L’élément FreeBusyResponse** contient les informations de libre/occupé d’un utilisateur de boîte aux lettres unique. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 **FreeBusyResponseType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> |Fournit des informations descriptives sur l’état de la réponse.  <br/> |
|[FreeBusyView](freebusyview.md) <br/> |Contient des informations de disponibilité pour un utilisateur spécifique.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FreeBusyResponseArray](freebusyresponsearray.md) <br/> |Contient les informations de disponibilité des utilisateurs demandés et l’état de la réponse.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas inclus dans une réponse GetUserAvailability si aucune information de disponibilité n’est demandée.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetUserAvailability](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

