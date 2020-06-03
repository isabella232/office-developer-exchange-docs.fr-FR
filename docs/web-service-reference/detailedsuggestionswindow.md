---
title: DetailedSuggestionsWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DetailedSuggestionsWindow
api_type:
- schema
ms.assetid: 7b348d63-6a7d-45f4-9562-5c42243d63a5
description: L’élément DetailedSuggestionsWindow identifie l’intervalle de temps interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées.
ms.openlocfilehash: 45d582f2642c0e3d8f6330b09946230c8842618d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467843"
---
# <a name="detailedsuggestionswindow"></a>DetailedSuggestionsWindow

L’élément **DetailedSuggestionsWindow** identifie l’intervalle de temps interrogé pour obtenir des informations détaillées sur les heures de réunion suggérées. 
  
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
|[StartTime](starttime.md) <br/> |Représente le début de la période interrogée pour obtenir des informations détaillées sur les heures de réunion suggérées.  <br/> |
|[EndTime](endtime.md) <br/> |Représente la fin de la période interrogée pour obtenir des informations détaillées sur les heures de réunion suggérées.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |Contient les options permettant d’obtenir des informations sur les suggestions de réunion.  <br/> Voici le XPath de cet élément :  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément n’est pas obligatoire.
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire/EWS/de l’ordinateur exécutant MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé. 
  
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

