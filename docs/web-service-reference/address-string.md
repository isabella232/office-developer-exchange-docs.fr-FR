---
title: Address (String)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Address
api_type:
- schema
ms.assetid: a3cdfcbd-d0c5-46d6-8daa-52405fc63ff0
description: L’élément Address représente l’adresse de messagerie de l’utilisateur de boîte aux lettres.
ms.openlocfilehash: a3648246b6be8c4f7d6421fc979a57e782ef3598
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543799"
---
# <a name="address-string"></a>Address (String)

**L’élément Address** représente l’adresse de messagerie de l’utilisateur de boîte aux lettres. 
  
```xml
<Address>...</Address>
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
|[Email (EmailAddressType)](email-emailaddresstype.md) <br/> |Spécifie l’adresse de messagerie de l’objet MailboxData. Cet élément est utilisé dans [l’opération GetUserAvailability](getuseravailability-operation.md).<br/><br/> Voici le chemin d’accès XPath à cet élément :<br/><br/>  `/GetUserAvailabilityRequest/MailboxDataArray/MailboxData[i]/Email` <br/> |
|[Mailbox (Availability)](mailbox-availability.md) <br/> | Représente l’utilisateur de boîte aux lettres pour une demande SetUserOofSettings ou GetUserOofSettings.<br/><br/>  Les expressions XPath de cet élément sont les suivantes :<br/><br/>  `/GetUserOofSettingsRequest/Mailbox` <br/>  `/SetUserOofSettingsRequest/Mailbox` <br/> |
   
## <a name="text-value"></a>Valeur texte

Une valeur de texte est requise si cet élément est utilisé.
  
## <a name="remarks"></a>Remarques

Cet élément peut se produire au plus une fois dans l’élément [Email (EmailAddressType)](email-emailaddresstype.md) et l’élément [Mailbox (Availability).](mailbox-availability.md) 
  
> [!NOTE]
> Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé. 
  
## <a name="element-information"></a>Informations sur l'élément

|||
|:-----|:-----|
|Espace de noms  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Nom du schéma  <br/> |Schéma Types  <br/> |
|Fichier de validation  <br/> |Types.xsd  <br/> |
|Peut être vide  <br/> |False  <br/> |
   
## <a name="see-also"></a>Voir aussi

- [Opération GetUserAvailability](getuseravailability-operation.md)
- [Opération GetUserOofSettings](getuseroofsettings-operation.md)
- [Opération SetUserOofSettings](setuseroofsettings-operation.md)
- [GetUserAvailabilityRequest](getuseravailabilityrequest.md)
- [GetUserOofSettingsRequest](getuseroofsettingsrequest.md)
- [SetUserOofSettingsRequest](setuseroofsettingsrequest.md)
- [Obtention de la disponibilité des utilisateurs](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

