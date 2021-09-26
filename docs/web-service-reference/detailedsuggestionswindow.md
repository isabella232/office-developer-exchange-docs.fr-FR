---
title: DetailedSuggestionsWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DetailedSuggestionsWindow
api_type:
- schema
ms.assetid: 7b348d63-6a7d-45f4-9562-5c42243d63a5
description: L’élément DetailedSuggestionsWindow identifie l’étendue de temps qui est interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées.
ms.openlocfilehash: 56f66d9ee7be25de20a892823a02174c75b40601
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545334"
---
# <a name="detailedsuggestionswindow"></a>DetailedSuggestionsWindow

**L’élément DetailedSuggestionsWindow** identifie l’étendue de temps qui est interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées. 
  
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md) 
- [SuggestionsViewOptions](suggestionsviewoptions.md) 
- [DetailedSuggestionsWindow](detailedsuggestionswindow.md)
  
```xml
<DetailedSuggestionsWindow>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
</DetailedSuggestionsWindow>
```

 **Duration**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |Représente le début de l’étendue de temps pour obtenir des informations détaillées sur les heures de réunion suggérées.  <br/> |
|[EndTime](endtime.md) <br/> |Représente la fin de l’étendue de temps pour obtenir des informations détaillées sur les heures de réunion suggérées.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contient les options pour obtenir des informations sur les suggestions de réunion.  <br/> Voici le chemin d’accès XPath à cet élément :  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas requis.
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire /EWS/ de l’ordinateur qui exécute MicrosoftExchange Server 2007 sur qui le rôle serveur d’accès au client est installé. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

