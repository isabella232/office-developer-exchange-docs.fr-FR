---
title: Présentateurs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: L’élément de présentateurs spécifie les présentateurs pour une réunion en ligne.
ms.openlocfilehash: f62b458759e0d8199c98827602d6c3fe16aebeea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828875"
---
# <a name="presenters"></a>Présentateurs

L’élément de **Présentateurs** spécifie les présentateurs pour une réunion en ligne. 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 **PresentersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte d’élément de **Présentateurs** est le type d’utilisateurs qui peut être un présentateur pour une réunion en ligne. Les valeurs de texte de l’élément **Présentateurs** sont décrits dans le tableau suivant. 
  
**Valeurs de texte des éléments présentateurs**

|**Valeur**|**Description**|
|:-----|:-----|
|Désactivé  <br/> |Les présentateurs sont désactivées.  <br/> |
|Interne  <br/> |Seuls les participants internes peuvent être présentateurs.  <br/> |
|Tout le monde  <br/> |N’importe quel participant peut être un présentateur.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013.
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> ||
   

