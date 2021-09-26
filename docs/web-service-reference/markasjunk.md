---
title: MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f06bafc6-7ee3-4b2b-9fd1-7c51328f4729
description: L’élément MarkAsJunk spécifie la demande de déplacement d’un élément vers le dossier de courrier indésirable et d’ajout de l’expéditeur à la liste des expéditeurs bloqués.
ms.openlocfilehash: 252c36b8bb3662ffd6c0fe470a81b6f0b55acb69
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544086"
---
# <a name="markasjunk"></a>MarkAsJunk

**L’élément MarkAsJunk** spécifie la demande de déplacement d’un élément vers le dossier de courrier indésirable et d’ajout de l’expéditeur à la liste des expéditeurs bloqués. 
  
```XML
<MarkAsJunk IsJunk="true | false" MoveItem="true | false">
   <ItemIds/>
</MarkAsJunk>
```

 **MarkAsJunkType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

|**Attribut**|**Description**|
|:-----|:-----|
|IsJunk  <br/> |Une valeur de texte **true** pour l’attribut **IsJunk** indique que l’expéditeur de courrier électronique est ajouté à la liste des expéditeurs bloqués. La valeur **false** indique que l’expéditeur du courrier électronique est supprimé de la liste des expéditeurs bloqués, si l’expéditeur de messagerie figure déjà dans la liste.  <br/> |
|MoveItem  <br/> |Une valeur de texte **true** pour l’attribut **MoveItem** indique que l’élément est déplacé vers le dossier de courrier indésirable par défaut. La valeur **false indique** que l’élément n’est pas déplacé vers le dossier de courrier indésirable par défaut.  <br/> |
   
### <a name="child-elements"></a>Éléments enfants

[ItemIds](itemids.md)
  
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |messages.xsd  <br/> |
|Peut être vide  <br/> ||
   

