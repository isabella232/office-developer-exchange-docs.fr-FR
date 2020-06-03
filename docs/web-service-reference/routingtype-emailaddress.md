---
title: RoutingType (EmailAddress)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoutingType
api_type:
- schema
ms.assetid: 74d83198-0d9d-4c78-a2bc-9a671859ff37
description: L’élément RoutingType représente le protocole de routage pour le destinataire.
ms.openlocfilehash: 2193e72c38c687669f6e052b4d2526029aa89d89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459033"
---
# <a name="routingtype-emailaddress"></a>RoutingType (EmailAddress)

L’élément **RoutingType** représente le protocole de routage pour le destinataire. 
  
```XML
<RoutingType/>
```

 **chaîne**
## <a name="attributes-and-elements"></a>Attributs et éléments

Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.
  
### <a name="attributes"></a>Attributs

Aucune.
  
### <a name="child-elements"></a>Éléments enfants

Aucun.
  
### <a name="parent-elements"></a>Éléments parents

|**Élément**|**Description**|
|:-----|:-----|
|[E-mail (EmailAddressType)](email-emailaddresstype.md) <br/> |Spécifie l’adresse de messagerie de l’objet MailboxData. Cet élément est utilisé dans l' [opération GetUserAvailability](getuseravailability-operation.md).  <br/><br/> Voici le XPath de cet élément :  <br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Boîte aux lettres (disponibilité)](mailbox-availability.md) <br/> | Représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.  <br/><br/>  Voici les expressions XPath de cet élément : <br/> <br/>  `/GetUserOofSettingsRequest/Mailbox` <br/><br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est facultative. Les valeurs possibles sont les suivantes :

* SMTP
* EX

Si aucune valeur n’est fournie, la valeur par défaut SMTP est utilisée.
  
## <a name="remarks"></a>Remarques

Cet élément peut apparaître au plus une fois dans l’élément [email (EmailAddressType)](email-emailaddresstype.md) . Cet élément n’est pas obligatoire. Cet élément existe pour l’inclusion des futurs protocoles. Un autre élément **RoutingType** est utilisé pour accéder aux éléments de la boîte aux lettres d’un utilisateur. 
  
Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

