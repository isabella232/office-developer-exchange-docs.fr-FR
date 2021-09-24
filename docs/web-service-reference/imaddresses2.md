---
title: ImAddresses2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 328f29b9-3a9c-4d9a-a85f-5ffff84e266a
description: L’élément ImAddresses2 spécifie un tableau d’adresses de message instantané et les identificateurs de leurs attributions source pour le personnage associé.
ms.openlocfilehash: aaad3fba834d8793328d2e4de061880f073f6971
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515683"
---
# <a name="imaddresses2"></a>ImAddresses2

**L’élément ImAddresses2** spécifie un tableau d’adresses de message instantané et les identificateurs de leurs attributions source pour le personnage associé. 
  
```XML
<ImAddresses2>
    <StringAttributedValue/>
</ImAddresses2>
```

 **ArrayOfStringAttributedValuesType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[StringAttributedValue](stringattributedvalue.md) <br/> |Spécifie une instance dans un tableau d’attributs associés à un élément persona.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Persona](persona.md) <br/> |Spécifie un ensemble de données de personnage renvoyées par une **demande GetPersona.**  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types.xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

