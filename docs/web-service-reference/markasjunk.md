---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: L’élément MarkAsJunk spécifie la demande pour déplacer un élément vers le dossier courrier indésirable et d’ajouter l’expéditeur à la liste des expéditeurs bloqués.
ms.openlocfilehash: fbb3eee7ce350954888931ca55b27f596656b161
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19828350"
---
# <a name="markasjunk"></a>MarkAsJunk

L’élément **MarkAsJunk** spécifie la demande pour déplacer un élément vers le dossier courrier indésirable et d’ajouter l’expéditeur à la liste des expéditeurs bloqués. 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 **MarkAsJunkType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|IsJunk  <br/> |Une valeur de texte de **la valeur true** pour l’attribut **IsJunk** indique que l’expéditeur est ajouté à la liste des expéditeurs bloqués. La valeur **false** indique que l’expéditeur est supprimé de la liste des expéditeurs bloqués, si l’expéditeur figure déjà dans la liste.  <br/> |
|MoveItem  <br/> |Une valeur de texte de **la valeur true** pour l’attribut **MoveItem** indique que l’élément est déplacé vers le dossier de courrier indésirable par défaut. La valeur **false** indique que l’élément n’est pas déplacé vers le dossier de courrier indésirable par défaut.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

[ItemId](itemids.md)
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

