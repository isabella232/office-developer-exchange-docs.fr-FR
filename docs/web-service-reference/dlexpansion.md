---
title: DLExpansion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DLExpansion
api_type:
- schema
ms.assetid: 9e50278d-fe6a-45e2-a72b-0fb06809e128
description: L’élément DLExpansion contient un tableau de boîtes aux lettres qui sont contenus dans une liste de distribution.
ms.openlocfilehash: 06081b4aba761a7137f921b3bc1c8d6b2afab88c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756025"
---
# <a name="dlexpansion"></a>DLExpansion

L’élément **DLExpansion** contient un tableau de boîtes aux lettres qui sont contenus dans une liste de distribution. 
  
- [ExpandDLResponse](expanddlresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
- [DLExpansion](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 **ArrayOfDLExpansionType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Représente l’index suivant doit être utilisé pour la requête suivante lorsque vous utilisez un affichage de page indexés.  <br/> |
|**NumeratorOffset** <br/> |Représente la nouvelle valeur numérateur à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.  <br/> |
|**AbsoluteDenominator** <br/> |Représente le dénominateur suivant à utiliser pour la requête suivante lorsque vous utilisez des affichages de page de fraction.  <br/> |
|**IncludesLastItemInRange** <br/> |Indique si les résultats actuels contient le dernier élément dans la requête afin que le fichier d’échange supplémentaire n’est pas nécessaire.  <br/> |
|**TotalItemsInView** <br/> |Représente le nombre total d’éléments dans l’affichage.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[Boîte aux lettres](mailbox.md) <br/> |Identifie un objet de service d'annuaire à extension messagerie Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Contient l’état et les résultats d’une seule demande ExpandDL.  <br/> |
   
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération ExpandDL](expanddl-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md) 
- [Référence EWS pour Exchange](ews-reference-for-exchange.md)

