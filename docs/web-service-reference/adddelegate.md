---
title: AddDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AddDelegate
api_type:
- schema
ms.assetid: 646fb994-229e-4d90-8b95-6541191cb3ae
description: L’élément AddDelegate définit une demande d’ajout de délégués à une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a08b83ad6e114c194073716c82228ea20ae1d3b7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466499"
---
# <a name="adddelegate"></a>AddDelegate

L’élément **AddDelegate** définit une demande d’ajout de délégués à une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1). 
  
```xml
<AddDelegate>
   <DelegateUsers/>
   <DeliverMeetingRequests/>
   <Mailbox/>
</AddDelegate>
```

 **AddDelegateType**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

|**Élément**|**Description**|
|:-----|:-----|
|[DelegateUsers](delegateusers.md) <br/> |Contient les identités des délégués à ajouter à ou à mettre à jour dans une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[DeliverMeetingRequests](delivermeetingrequests.md) <br/> |Définit la manière dont les demandes de réunion sont gérées entre le délégué et le principal. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).  <br/> |
|[Boîte aux lettres](mailbox.md) <br/> |Identifie un objet de service d'annuaire à extension messagerie Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Éléments parents

Aucun.
  
## <a name="remarks"></a>Remarques

Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Nom du schéma  <br/> |Schéma Messages  <br/> |
|Fichier de validation  <br/> |Messages. xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération AddDelegate](adddelegate-operation.md)
- [Éléments XML de EWS dans Exchange](ews-xml-elements-in-exchange.md)
- [Ajout de délégués](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

