---
title: Identifier le compte pour emprunter l’identité
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: Découvrez comment votre application de service utilise EWS pour identifier l’utilisateur pour emprunter l’identité.
ms.openlocfilehash: 78df4b511a9947d4d815b2802a53ab178b14622b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19754841"
---
# <a name="identify-the-account-to-impersonate"></a>Identifier le compte pour emprunter l’identité

Découvrez comment votre application de service utilise EWS pour identifier l’utilisateur pour emprunter l’identité.
  
Votre application de service identifie le compte d’utilisateur pour emprunter l’identité à l’aide d’un des trois identificateurs suivants :
  
- L’adresse SMTP principale.
    
- Le nom principe d’utilisateur (UPN).
    
- L’identificateur de sécurité (SID).
    
L’identificateur que vous utilisez dépend, bien sûr, les informations que votre application est disponible.
  
## <a name="identifying-the-user-account-to-impersonate"></a>Identifier le compte d’utilisateur pour emprunter l’identité

Votre application peut utiliser les demandes SOAP EWS ou API managées pour identifier le compte d’utilisateur qui il emprunte l’identité. L’API managée EWS utilise la propriété [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) pour identifier l’emprunt d’identité utilisateur. EWS utilise l’élément [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , comme illustré dans le fragment XML suivant. 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

Chacune des sections ci-dessous montre comment utiliser un des identificateurs. Pour obtenir un exemple qui illustre l’identificateur de l’emprunt d’identité en action, voir [Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a>Utiliser l’adresse de messagerie SMTP pour identifier le compte d’utilisateur

L’adresse de messagerie SMTP est l’adresse de messagerie principale qui est associé à un compte d’utilisateur.
  
Dans une application d’API managées, vous spécifiez l’adresse de messagerie SMTP ainsi que la valeur d’énumération [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

Dans une demande SOAP EWS, l’élément [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) contient l’adresse de messagerie pour le compte d’utilisateur. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a>L’UPN permet d’identifier le compte d’utilisateur

L’UPN contient le nom de domaine complet (FQDN) pour l’emplacement du compte d’utilisateur. Ce n’est pas nécessairement domaine de boîte aux lettres de l’utilisateur. L’attribut **UserPrincipleName** doit être correctement définie sur le compte d’utilisateur dans les Services de domaine Active Directory (AD DS) pour la recherche de l’utilisateur aboutisse. 
  
Dans une application d’API managées, vous spécifiez l’UPN ainsi que la valeur d’énumération [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

Dans une demande SOAP EWS, le [au PrincipalName, élément (ConnectingSIDType, complexType) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx) élément contient l’UPN du compte d’utilisateur. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a>Utiliser le SID pour identifier le compte d’utilisateur

Le SID est l’identificateur du compte pour être représenté dans le formulaire de sécurité descripteur definition language (SDDL).
  
Dans une application API managée EWS, vous spécifiez le SID ainsi que la valeur d’énumération [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

Dans une demande SOAP EWS, l’élément [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) contient l’identificateur de sécurité pour le compte d’utilisateur. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a>Voir aussi


- [Emprunt d'identité et EWS dans Exchange](impersonation-and-ews-in-exchange.md)
    
- [Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [Classe de ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

