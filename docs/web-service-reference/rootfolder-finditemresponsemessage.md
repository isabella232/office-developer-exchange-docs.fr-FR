---
title: RootFolder (FindItemResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: L’élément RootFolder contient les résultats d’une recherche d’un dossier racine unique au cours d’une opération FindItem.
ms.openlocfilehash: 96fa9e162dde34394e7c34543dd25a6f018ae7de
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527536"
---
# <a name="rootfolder-finditemresponsemessage"></a>RootFolder (FindItemResponseMessage)

**L’élément RootFolder** contient les résultats d’une recherche d’un dossier racine unique au cours d’une [opération FindItem](finditem-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 **FindItemParentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Représente l’index suivant qui doit être utilisé pour la demande suivante lors de l’utilisation d’une vue de pagination indexée.  <br/> |
|**NumeratorOffset** <br/> |Représente la nouvelle valeur de numérateur à utiliser pour la demande suivante lors de l’utilisation d’affichages de page de fraction.  <br/> |
|**AbsoluteDenominator** <br/> |Représente le dénominateur suivant à utiliser pour la demande suivante lors de la pagination fractionnaire.  <br/> |
|**IncludesLastItemInRange** <br/> |Indique si les résultats actuels contiennent le dernier élément de la requête, de telles que la pagination supplémentaire n’est pas nécessaire.  <br/> |
|**TotalItemsInView** <br/> |Représente le nombre total d’éléments qui passent la restriction. Dans une opération [FindItem](finditem-operation.md)groupée, l’attribut **TotalItemsInView** renvoie le nombre total d’éléments dans l’affichage plus le nombre total de groupes.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Items](items.md) <br/> |Contient un tableau d’éléments trouvés dont les critères de recherche sont identifiés dans la [demande d’opération FindItem.](finditem-operation.md)  <br/> |
|[Groupes](groups.md) <br/> |Contient une collection de groupes trouvés dont les critères de recherche et d’agrégation sont identifiés dans la [demande d’opération FindItem.](finditem-operation.md)  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindItemResponseMessage](finditemresponsemessage.md) <br/> |Contient l’état et le résultat [d’une demande d’opération FindItem.](finditem-operation.md)  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Exchange Server avec le rôle serveur d’accès au client installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindItem](finditem-operation.md)
  
[IndexedPagingOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[NumeratorOffset](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[AbsoluteDenominator](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[IncludesLastItemInRange](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[TotalItemsInView](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[Recherche d’éléments](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

