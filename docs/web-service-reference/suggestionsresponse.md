---
title: SuggestionsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionsResponse
api_type:
- schema
ms.assetid: d25ca143-f80c-4458-b669-346fda29a5a7
description: L’élément SuggestionsResponse contient des informations sur l’état de réponse et des données de suggestion pour les suggestions de réunion demandées.
ms.openlocfilehash: 92dfac3cc0a6ddce9485a8cb266f072795b18bd5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544527"
---
# <a name="suggestionsresponse"></a>SuggestionsResponse

**L’élément SuggestionsResponse** contient des informations sur l’état de réponse et des données de suggestion pour les suggestions de réunion demandées. 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 **SuggestionsResponseType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[ResponseMessage](responsemessage.md) <br/> |Fournit des informations descriptives sur l’état de la réponse.  <br/> |
|[SuggestionDayResultArray](suggestiondayresultarray.md) <br/> |Contient un tableau de suggestions de réunion organisées par date.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetUserAvailabilityResponse](getuseravailabilityresponse.md) <br/> |Contient les informations de disponibilité des utilisateurs demandés.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas inclus dans une réponse GetUserAvailability si [SuggestionsViewOptions n’est](suggestionsviewoptions.md) pas définie dans le message de demande GetUserAvailability. 
  
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

