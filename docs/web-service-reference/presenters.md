---
title: Présentateurs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: L’élément Presenters spécifie les présentateurs pour une réunion en ligne.
ms.openlocfilehash: 1c9bf9093450e675245b647c98d7b1d00101ce9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519141"
---
# <a name="presenters"></a>Présentateurs

**L’élément Presenters** spécifie les présentateurs d’une réunion en ligne. 
  
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

La valeur de texte **de l’élément Presenters** est le type d’utilisateurs qui peuvent être présentateurs d’une réunion en ligne. Les valeurs de texte de **l’élément Presenters** sont décrites dans le tableau suivant. 
  
**Valeurs de texte de l’élément Presenters**

|**Valeur**|**Description**|
|:-----|:-----|
|Désactivé  <br/> |Les présentateurs sont désactivés.  <br/> |
|Interne  <br/> |Seuls les participants internes peuvent être présentateurs.  <br/> |
|Tout le monde  <br/> |N’importe quel participant peut être présentateur.  <br/> |
   
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
   

