---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: La valeur de l’élément AppStatus indique l’état de l’application de messagerie.
ms.openlocfilehash: cf213fc3d7be02c411e9c2e83a4ff153dbefe098
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755311"
---
# <a name="appstatus"></a>AppStatus

La valeur de l’élément **AppStatus** indique l’état de l’application de messagerie. 
  
```XML
<AppStatus/>
```

 **string**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Métadonnées](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a>Valeur de texte

La valeur de texte de l’élément **AppStatus** indique l’état de l’application de messagerie. Si l’utilisateur peut résoudre un problème lié à l’état de l’application de messagerie, l’élément [ActionUrl](actionurl.md) fournit l’URL pour effectuer le correctif. 
  
**Le tableau 1. Valeurs AppStatus**

|**Valeur**|**Description**|
|:-----|:-----|
|NULL ou 0  <br/> |L’application de messagerie a un état sain.  <br/> |
|1.0  <br/> |L’application de messagerie n’a pas pu être chargée automatiquement. L’application de messagerie doit être installée à partir de l’Office Store.  <br/> |
|1.1  <br/> |L’application de messagerie n’a pas pu être chargée automatiquement. L’application de messagerie nécessite des autorisations accrues, mais ceci nécessite votre révision et confirmer l’installation.  <br/> |
|1.2  <br/> |L’application de messagerie n’a pas pu être mis à jour automatiquement. La licence actuelle a expiré ou n’est pas valide. Mettez à jour l’application de messagerie de l’Office Store.  <br/> |
|2.0  <br/> |La licence d’application de messagerie n’a pas pu être chargée automatiquement. La licence pour l’application de messagerie doit être récupéré à partir de l’Office Store.  <br/> |
|2.1  <br/> |La licence d’application de messagerie n’a pas pu être chargée automatiquement. La licence actuelle a expiré. Une nouvelle licence pour cette application doit être installé à partir de l’Office Store.  <br/> |
|3.0  <br/> |L’état de l’Office Store pour l’application de messagerie a changé. Cela peut indiquer qu’il existe un problème avec l’application de messagerie. Accédez à la page d’application de messagerie dans l’Office Store pour plus d’informations.  <br/> |
|3.1  <br/> |L’application de messagerie a été supprimée de l’Office Store.  <br/> |
|3.2  <br/> |Un problème a été détecté avec l’application de messagerie et il a été temporairement retiré de l’Office Store.  <br/> |
|3.3  <br/> |L’application de messagerie sera supprimée du magasin de bureau dans les 30 jours.  <br/> |
|4.0  <br/> |L’application de messagerie a été désactivée automatiquement par votre client de messagerie.  <br/> |
|4.1  <br/> |L’application de messagerie a été désactivée par Outlook pour des raisons de performances.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> | http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Not applicable  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Métadonnées](metadata-ex15websvcsotherref.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

