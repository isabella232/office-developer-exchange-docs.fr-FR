---
title: Présentateurs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: L’élément Presenters spécifie les présentateurs d’une réunion en ligne.
ms.openlocfilehash: 0236457020dfc4684569e84d3d54e357af00d102
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529909"
---
# <a name="presenters"></a>Présentateurs

L’élément **Presenters** spécifie les présentateurs d’une réunion en ligne. 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 **PresentersType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[OnlineMeetingSettings](onlinemeetingsettings.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de l’élément **Presenters** est le type d’utilisateurs pouvant être présentateur pour une réunion en ligne. Les valeurs de texte de l’élément **Presenters** sont décrites dans le tableau suivant. 
  
**Valeurs de texte de l’élément Presenters**

|**Valeur**|**Description**|
|:-----|:-----|
|Désactivé  <br/> |Les présentateurs sont désactivés.  <br/> |
|Interne  <br/> |Seuls les participants internes peuvent être présentateurs.  <br/> |
|Tout le monde  <br/> |Tout participant peut être présentateur.  <br/> |
   
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
   

