---
title: ResolutionSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: L’élément ResolutionSet contient un tableau de résolutions pour un nom ambigu.
ms.openlocfilehash: f77b8a94871aa7827c98a3bb15fdf4a3a35c7c55
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521745"
---
# <a name="resolutionset"></a>ResolutionSet

**L’élément ResolutionSet** contient un tableau de résolutions pour un nom ambigu. 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Représente l’index suivant qui doit être utilisé pour la requête suivante lorsque vous utilisez un affichage de page indexé.  <br/> |
|**NumeratorOffset** <br/> |Représente la nouvelle valeur de numérateur à utiliser pour la demande suivante lorsque vous utilisez des affichages de page de fraction.  <br/> |
|**AbsoluteDenominator** <br/> |Représente le dénominateur suivant à utiliser pour la requête suivante lorsque vous utilisez des vues de page de fraction.  <br/> |
|**IncludesLastItemInRange** <br/> |Cet attribut aura la valeur true si les résultats actuels contiennent le dernier élément de la requête, de sorte que la pagination supplémentaire n’est pas nécessaire.  <br/> |
|**TotalItemsInView** <br/> |Représente le nombre total d’éléments dans l’affichage.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Solution](resolution.md) <br/> |Contient une seule entité résolue.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ResolveNamesResponseMessage](resolvenamesresponsemessage.md) <br/> |Contient l’état et le résultat d’une demande ResolveNames.  <br/> |
   
## <a name="remarks"></a>Remarques

Un **élément ResolutionSet** peut contenir un maximum de 100 entités résolues. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[ResolveNames](resolvenames.md)
  
[ResolveNamesResponse](resolvenamesresponse.md)
  
[Opération ResolveNames](resolvenames-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

