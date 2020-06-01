---
title: ImAddresses2
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 328f29b9-3a9c-4d9a-a85f-5ffff84e266a
description: L’élément ImAddresses2 spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions sources pour le personnage associé.
ms.openlocfilehash: b2a9f61ba31c1324ac5563bb6ab6b30f0271c653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460763"
---
# <a name="imaddresses2"></a>ImAddresses2

L’élément **ImAddresses2** spécifie un tableau d’adresses de messagerie instantanée et les identificateurs de leurs attributions sources pour le personnage associé. 
  
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
|[StringAttributedValue](stringattributedvalue.md) <br/> |Spécifie une instance dans un tableau d’attributs associés à un élément Persona.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Persona](persona.md) <br/> |Spécifie un ensemble de données Persona renvoyées par une demande **GetPersona** .  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma type  <br/> |
|Validation File  <br/> |types. xsd  <br/> |
|Peut être vide  <br/> ||
   
## <a name="see-also"></a>Voir aussi



- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

