---
title: ItemShape
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: L’élément ItemShape identifie un ensemble de propriétés à retourner dans une opération GetItem, FindItem opération ou une réponse d’opération SyncFolderItems.
ms.openlocfilehash: 95174a85a8fa05cb2612e1289d46c8db32b6e052
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828191"
---
# <a name="itemshape"></a>ItemShape

L’élément **ItemShape** identifie un ensemble de propriétés à retourner dans une réponse [GetItem operation](getitem-operation.md), [opération FindItem](finditem-operation.md)ou [SyncFolderItems](syncfolderitems-operation.md) . 
  
```XML
<ItemShape>
   <BaseShape/>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <ConvertHtmlCodePageToUTF8/>
   <AdditionalProperties/>
</ItemShape>
```

 **ItemResponseShapeType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |Identifie la configuration de propriétés à retourner dans une réponse de l’élément ou le dossier de base.  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |Spécifie si le contenu Multipurpose Internet Mail Extensions (MIME) d’un élément est renvoyé dans la réponse.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifie la mise en forme le corps du texte dans la réponse.  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |Indique si l’élément corps HTML est converti en UTF-8.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Spécifie si le filtrage du contenu HTML est activé.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifie les propriétés supplémentaires pour retourner une réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Définit une requête pour récupérer des éléments à partir d’une boîte aux lettres dans la banque d’informations Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher tous les éléments contenus dans un dossier.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.  <br/> Vous trouverez ci-dessous l’expression XPath pour cet élément :  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[GetItem Operation](getitem-operation.md)
  
[Opération FindItem](finditem-operation.md)
  
[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

