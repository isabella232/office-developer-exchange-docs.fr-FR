---
title: Identifier le compte d’emprunt d’identité
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: c7749f12-b97f-48d9-88e5-a545e108efb0
description: Découvrez comment votre application de service utilise EWS pour identifier l’utilisateur à emprunter.
localization_priority: Priority
ms.openlocfilehash: 7159707abe96632aba2ed70dc0057417e087349f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527991"
---
# <a name="identify-the-account-to-impersonate"></a>Identifier le compte d’emprunt d’identité

Découvrez comment votre application de service utilise EWS pour identifier l’utilisateur à emprunter.
  
Votre application de service identifie le compte d’utilisateur dont l’identité doit être empruntée à l’aide de l’un des trois identificateurs suivants :
  
- Adresse SMTP principale.
    
- Nom d’utilisateur principal (UPN).
    
- Identificateur de sécurité (SID).
    
L’identificateur que vous utilisez dépend, bien sûr, des informations que votre application est disponible.
  
## <a name="identifying-the-user-account-to-impersonate"></a>Identification du compte d’utilisateur dont l’identité doit être empruntée

Votre application peut utiliser l’API managée EWS ou les requêtes SOAP EWS pour identifier le compte d’utilisateur dont elle emprunte l’identité. L’API managée EWS utilise la propriété [ExchangeService. ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) pour identifier l’utilisateur emprunté. EWS utilise l’élément [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , comme illustré dans le fragment XML suivant. 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

Chacune des sections suivantes indique comment utiliser l’un des identificateurs. Pour obtenir un exemple qui montre l’identificateur d’emprunt d’identité en action, consultez la rubrique [Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a>Utiliser l’adresse de messagerie SMTP pour identifier le compte d’utilisateur

L’adresse de messagerie SMTP est l’adresse de messagerie principale associée à un compte d’utilisateur.
  
Dans une application d’API managée EWS, vous spécifiez l’adresse de messagerie SMTP avec la valeur d’énumération [ConnectingIdType. SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

Dans une demande EWS SOAP, l’élément [PrimarySmtpAddress](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) contient l’adresse de messagerie du compte d’utilisateur. 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a>Utiliser le nom d’utilisateur principal pour identifier le compte d’utilisateur

L’UPN contient le nom de domaine complet (FQDN) de l’emplacement du compte d’utilisateur. Il ne s’agit pas nécessairement du domaine de boîte aux lettres de l’utilisateur. L’attribut **userPrincipalName** doit être correctement défini sur le compte d’utilisateur dans les services de domaine Active Directory (AD DS) pour que la recherche de l’utilisateur réussisse. 
  
Dans une application d’API managée EWS, vous spécifiez l’UPN avec la valeur d’énumération [ConnectingIdType. PrincipalName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipalName, "alias@billing.contoso.com");
```

Dans une demande EWS SOAP, l’élément [PrincipalName Element (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) contient l’UPN du compte d’utilisateur. 
  
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

Le SID est l’identificateur du compte sur lequel emprunter l’identité au format SDDL (Security Descriptor Definition Language).
  
Dans une application d’API managée EWS, vous spécifiez le SID avec la valeur d’énumération [ConnectingIdType. sid](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) . 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

Dans une demande de SOAP EWS, l’élément [sid](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) contient le SID du compte d’utilisateur. 
  
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
    
- [Classe de ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

