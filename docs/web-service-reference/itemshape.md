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
description: L’élément ItemShape identifie un jeu de propriétés à renvoyer dans une opération GetItem, FindItem ou SyncFolderItems.
ms.openlocfilehash: ffb666ee331b55a4f04cad076c705e4bec980e03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458123"
---
# <a name="itemshape"></a>ItemShape

L’élément **ItemShape** identifie un jeu de propriétés à renvoyer dans une [opération GetItem](getitem-operation.md), [FindItem](finditem-operation.md)ou [SyncFolderItems](syncfolderitems-operation.md) . 
  
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

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[BaseShape](baseshape.md) <br/> |Identifie la configuration de base des propriétés à renvoyer dans une réponse d’un élément ou d’un dossier.  <br/> |
|[IncludeMimeContent](includemimecontent.md) <br/> |Indique si le contenu MIME (Multipurpose Internet Mail Extensions) d’un élément est renvoyé dans la réponse.  <br/> |
|[BodyType](bodytype.md) <br/> |Identifie la façon dont le corps de texte est mis en forme dans la réponse.  <br/> |
|[ConvertHtmlCodePageToUTF8](converthtmlcodepagetoutf8.md) <br/> |Indique si le corps HTML de l’élément est converti en UTF8.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Indique si le filtrage du contenu HTML est activé.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Identifie les propriétés supplémentaires à renvoyer dans une réponse.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[GetItem](getitem.md) <br/> |Définit une demande de récupération des éléments d’une boîte aux lettres dans la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/GetItem` <br/> |
|[FindItem](finditem.md) <br/> |Définit une requête pour rechercher tous les éléments contenus dans un dossier.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/FindItem` <br/> |
|[SyncFolderItems](syncfolderitems.md) <br/> |Définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.  <br/> Voici l’expression XPath de cet élément :  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a>Valeur de texte

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi



[Opération GetItem](getitem-operation.md)
  
[Opération FindItem](finditem-operation.md)
  
[Opération SyncFolderItems](syncfolderitems-operation.md)


- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

