---
title: ImAddresses3
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cab51a28-dfad-4c70-aafe-e239321b784e
description: L’élément ImAddresses3 spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: 1d6ebf9d8e831f36ea7d947a72c60c58fa5b1a4a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827874"
---
# <a name="imaddresses3"></a>ImAddresses3

L’élément **ImAddresses3** spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions source pour le personnage associé. 
  
```XML
<ImAddresses3>
    <StringAttributedValue/>
</ImAddresses3>
```

 **ArrayOfStringAttributedValuesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[StringAttributedValue](stringattributedvalue.md) <br/> |Spécifie une instance d’un tableau d’attributs associés à un élément personnage.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Personnage](persona.md) <br/> |Spécifie un ensemble de données personnage renvoyées par une demande **GetPersona** .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

