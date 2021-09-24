---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: La valeur de l’élément AppStatus indique l’état de l’application de messagerie.
ms.openlocfilehash: 69f481b197db513761b97d4fbba38452bbb4a9a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525315"
---
# <a name="appstatus"></a>AppStatus

La **valeur de l’élément AppStatus** indique l’état de l’application de messagerie. 
  
```XML
<AppStatus/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

[Métadonnées](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a>Valeur texte

La valeur de texte de **l’élément AppStatus** indique l’état de l’application de messagerie. Si l’utilisateur peut résoudre un problème lié à l’état de l’application de messagerie, [l’élément ActionUrl](actionurl.md) fournit l’URL pour effectuer le correctif. 
  
**Tableau 1. Valeurs AppStatus**

|**Valeur**|**Description**|
|:-----|:-----|
|Null ou 0  <br/> |L’application de messagerie présente un état sain.  <br/> |
|1.0  <br/> |L’application de messagerie n’a pas pu être mise à jour automatiquement. L’application de messagerie doit être réinstallée à partir du Office Store.  <br/> |
|1.1  <br/> |L’application de messagerie n’a pas pu être mise à jour automatiquement. L’application de messagerie nécessite des autorisations accrues, ce qui nécessite votre révision et confirmation pour l’installation.  <br/> |
|1.2  <br/> |L’application de messagerie n’a pas pu être mise à jour automatiquement. La licence actuelle a expiré ou n’est pas valide. Veuillez mettre à jour l’application de messagerie à partir Office Store.  <br/> |
|2.0  <br/> |La licence de l’application de messagerie n’a pas pu être mise à jour automatiquement. La licence de l’application de messagerie doit être récupérée à partir du Office Store.  <br/> |
|2.1  <br/> |La licence de l’application de messagerie n’a pas pu être mise à jour automatiquement. La licence actuelle a expiré. Une nouvelle licence pour cette application doit être installée à partir du Office Store.  <br/> |
|3.0  <br/> |L Office’état de l’application de messagerie dans le Store a changé. Cela peut indiquer qu’il existe un problème avec l’application de messagerie. Pour plus d’informations, voir la page de l’application de messagerie Office Store.  <br/> |
|3.1  <br/> |L’application de messagerie a été supprimée du Office Store.  <br/> |
|3.2  <br/> |Un problème a été détecté avec l’application de messagerie et a été temporairement retiré du Office Store.  <br/> |
|3.3  <br/> |L’application de messagerie sera supprimée du Office Store dans un délai de 30 jours.  <br/> |
|4.0  <br/> |L’application de messagerie a été automatiquement désactivée par votre client de messagerie.  <br/> |
|4.1  <br/> |L’application de messagerie a été désactivée par Outlook pour des raisons de performances.  <br/> |
   
## <a name="remarks"></a>Remarques

Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> | https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Non applicable  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Métadonnées](metadata-ex15websvcsotherref.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)

