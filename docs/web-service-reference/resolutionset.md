---
title: ResolutionSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: L’élément ResolutionSet contient un tableau des résolutions pour un nom ambigu.
ms.openlocfilehash: ad7bd31c85051e8c80aea25aa9e6f2914cf0ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829160"
---
# <a name="resolutionset"></a>ResolutionSet

L’élément **ResolutionSet** contient un tableau des résolutions pour un nom ambigu. 
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[ResolveNamesResponseMessage](resolvenamesresponsemessage.md)
  
[ResolutionSet](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 **ArrayOfResolutionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Représente l’index suivant doit être utilisé pour la requête suivante lorsque vous utilisez un affichage de page indexés.  <br/> |
|**NumeratorOffset** <br/> |Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.  <br/> |
|**AbsoluteDenominator** <br/> |Représente le dénominateur suivant à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.  <br/> |
|**IncludesLastItemInRange** <br/> |Cet attribut sera la valeur true si le résultat actuel contient le dernier élément dans la requête, afin que le fichier d’échange supplémentaire n’est pas nécessaire.  <br/> |
|**TotalItemsInView** <br/> |Représente le nombre total d’éléments dans l’affichage.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Solution](resolution.md) <br/> |Contient une seule entité résolue.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’état et les résultats d’une demande ResolveNames.  <br/> |
   
## <a name="remarks"></a>Remarques

Un élément **ResolutionSet** peut contenir un maximum de 100 entités résolus. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[ResolveNames](resolvenames.md)
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[Opération ResolveNames](resolvenames-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

