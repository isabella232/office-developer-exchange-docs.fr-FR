---
title: DistinguishedUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedUser
api_type:
- schema
ms.assetid: 9362699d-666a-4acf-8fa1-c6669f0a2ae5
description: L’élément DistinguishedUser identifie les comptes d’utilisateurs par défaut et anonymes pour l’accès délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: b14be22bfe5316b9ab254e63cdfa0757596b8b92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756015"
---
# <a name="distinguisheduser"></a>DistinguishedUser

L’élément **DistinguishedUser** identifie les comptes d’utilisateurs par défaut et anonymes pour l’accès délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DistinguishedUser>Default or Anonymous</DistinguishedUser>
```

 **DistinguishedUserType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.
  
### <a name="attributes"></a>Attributs

Aucun.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[Nom d’utilisateur](userid.md) <br/> |Identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur de texte

Une valeur de texte **par défaut** décrit le paramètre par défaut pour les utilisateurs de délégué qui sont ajoutés à la boîte aux lettres de l’entité de sécurité. Une valeur texte **Anonymous** décrit les paramètres d’accès délégué que les utilisateurs anonymes sur boîte aux lettres de l’entité de sécurité. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération AddDelegate](adddelegate-operation.md)  
- [Opération UpdateDelegate](updatedelegate-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Ajout de délégués](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

