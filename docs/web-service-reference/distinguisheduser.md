---
title: DistinguishedUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DistinguishedUser
api_type:
- schema
ms.assetid: 9362699d-666a-4acf-8fa1-c6669f0a2ae5
description: L’élément DistinguishedUser identifie les comptes d’utilisateur anonyme et par défaut pour l’accès délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: ce59b5775f6f0516c469c7ee8bc4546780ce86d0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544240"
---
# <a name="distinguisheduser"></a>DistinguishedUser

**L’élément DistinguishedUser** identifie les comptes d’utilisateur anonyme et par défaut pour l’accès délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<DistinguishedUser>Default or Anonymous</DistinguishedUser>
```

 **DistinguishedUserType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[UserId](userid.md) <br/> |Identifie un utilisateur délégué ou un utilisateur qui dispose d’autorisations d’accès aux dossiers. Cet élément a été introduit dans Exchange 2007 SP1.  <br/> |
   
## <a name="text-value"></a>Valeur texte

La valeur de texte **Par** défaut décrit le paramètre par défaut pour les utilisateurs délégués qui sont ajoutés à la boîte aux lettres du principal. La valeur texte **Anonyme** décrit les paramètres d’accès délégué dont les utilisateurs anonymes ont sur la boîte aux lettres du principal. 
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération AddDelegate](adddelegate-operation.md)  
- [Opération UpdateDelegate](updatedelegate-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Ajout de délégués](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

