---
title: SearchScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4a53989e-eca6-45c4-afac-4d6ac19597d2
description: L’élément SearchScope spécifie l’étendue d’une recherche.
ms.openlocfilehash: d4caa87cd552a633812b99d7e97f2419b156fb78
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523398"
---
# <a name="searchscope"></a>SearchScope

**L’élément SearchScope** spécifie l’étendue d’une recherche. 
  
```XML
<SearchScope> PrimaryOnly | ArchiveOnly | All </SearchScope>
```

 **MailboxSearchLocationType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[MailboxSearchScope](mailboxsearchscope.md)
  
## <a name="text-value"></a>Valeur texte

La valeur texte de **l’élément SearchScope** indique le type de boîte aux lettres recherché pour une recherche de découverte. Une valeur de texte **PrimaryOnly indique** que la boîte aux lettres principale est recherché. La valeur texte **ArchiveOnly indique** que la boîte aux lettres d’archivage fait l’être. La valeur texte **All** indique que les boîtes aux lettres principale et d’archivage font l’être. 
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

