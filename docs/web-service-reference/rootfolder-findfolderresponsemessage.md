---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: L’élément RootFolder contient les résultats d’une recherche d’un dossier racine unique pendant une opération FindFolder.
ms.openlocfilehash: b5601d6abec67196c9991908e272a2122a201d69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457136"
---
# <a name="rootfolder-findfolderresponsemessage"></a>RootFolder (FindFolderResponseMessage)

L’élément **RootFolder** contient les résultats d’une recherche d’un dossier racine unique pendant une [opération FindFolder](findfolder-operation.md).
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 **FindFolderParentType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|IndexedPagingOffset  <br/> |Représente l’index suivant qui doit être utilisé pour la requête suivante lors de l’utilisation d’une vue de pagination indexée.  <br/> |
|NumeratorOffset  <br/> |Représente la nouvelle valeur de numérateur à utiliser pour la requête suivante lors de l’utilisation d’affichages de page fractionnaires.  <br/> |
|AbsoluteDenominator  <br/> |Représente le dénominateur suivant à utiliser pour la requête suivante lors de la pagination fractionnée.  <br/> |
|IncludesLastItemInRange  <br/> |Indique si les résultats actuels contiennent le dernier dossier de la requête, de sorte qu’aucune pagination supplémentaire n’est nécessaire.  <br/> |
|TotalItemsInView  <br/> |Représente le nombre total de dossiers qui ont passé la restriction.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Dossiers](folders-ex15websvcsotherref.md) <br/> |Contient un tableau de dossiers trouvés à l’aide de l' [opération FindFolder](findfolder-operation.md).  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[FindFolderResponseMessage](findfolderresponsemessage.md) <br/> |Contient l’État et le résultat d’une demande d' [opération FindFolder](findfolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server 2010 sur lequel le rôle de serveur d’accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération FindFolder](findfolder-operation.md)


[Recherche de dossiers](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

