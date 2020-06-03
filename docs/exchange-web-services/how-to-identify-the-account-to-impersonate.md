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
# <a name="identify-the-account-to-impersonate"></a><span data-ttu-id="1bf69-103">Identifier le compte d’emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="1bf69-103">Identify the account to impersonate</span></span>

<span data-ttu-id="1bf69-104">Découvrez comment votre application de service utilise EWS pour identifier l’utilisateur à emprunter.</span><span class="sxs-lookup"><span data-stu-id="1bf69-104">Learn how your service application uses EWS to identify the user to impersonate.</span></span>
  
<span data-ttu-id="1bf69-105">Votre application de service identifie le compte d’utilisateur dont l’identité doit être empruntée à l’aide de l’un des trois identificateurs suivants :</span><span class="sxs-lookup"><span data-stu-id="1bf69-105">Your service application identifies the user account to impersonate by using one of the following three identifiers:</span></span>
  
- <span data-ttu-id="1bf69-106">Adresse SMTP principale.</span><span class="sxs-lookup"><span data-stu-id="1bf69-106">The primary SMTP address.</span></span>
    
- <span data-ttu-id="1bf69-107">Nom d’utilisateur principal (UPN).</span><span class="sxs-lookup"><span data-stu-id="1bf69-107">The user principal name (UPN).</span></span>
    
- <span data-ttu-id="1bf69-108">Identificateur de sécurité (SID).</span><span class="sxs-lookup"><span data-stu-id="1bf69-108">The security identifier (SID).</span></span>
    
<span data-ttu-id="1bf69-109">L’identificateur que vous utilisez dépend, bien sûr, des informations que votre application est disponible.</span><span class="sxs-lookup"><span data-stu-id="1bf69-109">The identifier that you use depends, of course, on the information that your application has available.</span></span>
  
## <a name="identifying-the-user-account-to-impersonate"></a><span data-ttu-id="1bf69-110">Identification du compte d’utilisateur dont l’identité doit être empruntée</span><span class="sxs-lookup"><span data-stu-id="1bf69-110">Identifying the user account to impersonate</span></span>

<span data-ttu-id="1bf69-111">Votre application peut utiliser l’API managée EWS ou les requêtes SOAP EWS pour identifier le compte d’utilisateur dont elle emprunte l’identité.</span><span class="sxs-lookup"><span data-stu-id="1bf69-111">Your application can use either the EWS Managed API or EWS SOAP requests to identify the user account that it is impersonating.</span></span> <span data-ttu-id="1bf69-112">L’API managée EWS utilise la propriété [ExchangeService. ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) pour identifier l’utilisateur emprunté.</span><span class="sxs-lookup"><span data-stu-id="1bf69-112">The EWS Managed API uses the [ExchangeService.ImpersonatedUserId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property to identify the impersonated user.</span></span> <span data-ttu-id="1bf69-113">EWS utilise l’élément [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , comme illustré dans le fragment XML suivant.</span><span class="sxs-lookup"><span data-stu-id="1bf69-113">EWS uses the [ExchangeImpersonation](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) element, as shown in the following XML fragment.</span></span> 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

<span data-ttu-id="1bf69-114">Chacune des sections suivantes indique comment utiliser l’un des identificateurs.</span><span class="sxs-lookup"><span data-stu-id="1bf69-114">Each of the following sections shows how to use one of the identifiers.</span></span> <span data-ttu-id="1bf69-115">Pour obtenir un exemple qui montre l’identificateur d’emprunt d’identité en action, consultez la rubrique [Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).</span><span class="sxs-lookup"><span data-stu-id="1bf69-115">For an example that shows the impersonation identifier in action, see [Add appointments by using Exchange impersonation](how-to-add-appointments-by-using-exchange-impersonation.md).</span></span>
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a><span data-ttu-id="1bf69-116">Utiliser l’adresse de messagerie SMTP pour identifier le compte d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1bf69-116">Use the SMTP email address to identify the user account</span></span>

<span data-ttu-id="1bf69-117">L’adresse de messagerie SMTP est l’adresse de messagerie principale associée à un compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1bf69-117">The SMTP email address is the primary email address that is associated with a user account.</span></span>
  
<span data-ttu-id="1bf69-118">Dans une application d’API managée EWS, vous spécifiez l’adresse de messagerie SMTP avec la valeur d’énumération [ConnectingIdType. SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1bf69-118">In an EWS Managed API application, you specify the SMTP email address along with the [ConnectingIdType.SMTP](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

<span data-ttu-id="1bf69-119">Dans une demande EWS SOAP, l’élément [PrimarySmtpAddress](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) contient l’adresse de messagerie du compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1bf69-119">In an EWS SOAP request, the [PrimarySmtpAddress](https://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) element contains the email address for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a><span data-ttu-id="1bf69-120">Utiliser le nom d’utilisateur principal pour identifier le compte d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1bf69-120">Use the UPN to identify the user account</span></span>

<span data-ttu-id="1bf69-121">L’UPN contient le nom de domaine complet (FQDN) de l’emplacement du compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1bf69-121">The UPN contains the fully qualified domain name (FQDN) for the location of the user account.</span></span> <span data-ttu-id="1bf69-122">Il ne s’agit pas nécessairement du domaine de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1bf69-122">This is not necessarily the user's mailbox domain.</span></span> <span data-ttu-id="1bf69-123">L’attribut **userPrincipalName** doit être correctement défini sur le compte d’utilisateur dans les services de domaine Active Directory (AD DS) pour que la recherche de l’utilisateur réussisse.</span><span class="sxs-lookup"><span data-stu-id="1bf69-123">The **UserPrincipalName** attribute must be set correctly on the user account in Active Directory Domain Services (AD DS) for the user lookup to succeed.</span></span> 
  
<span data-ttu-id="1bf69-124">Dans une application d’API managée EWS, vous spécifiez l’UPN avec la valeur d’énumération [ConnectingIdType. PrincipalName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1bf69-124">In an EWS Managed API application, you specify the UPN along with the [ConnectingIdType.PrincipalName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipalName, "alias@billing.contoso.com");
```

<span data-ttu-id="1bf69-125">Dans une demande EWS SOAP, l’élément [PrincipalName Element (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) contient l’UPN du compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1bf69-125">In an EWS SOAP request, the [PrincipalName element (ConnectingSIDType complexType) (EWS)](../web-service-reference/principalname.md) element contains the UPN for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a><span data-ttu-id="1bf69-126">Utiliser le SID pour identifier le compte d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="1bf69-126">Use the SID to identify the user account</span></span>

<span data-ttu-id="1bf69-127">Le SID est l’identificateur du compte sur lequel emprunter l’identité au format SDDL (Security Descriptor Definition Language).</span><span class="sxs-lookup"><span data-stu-id="1bf69-127">The SID is the identifier of the account to be impersonated in security descriptor definition language (SDDL) form.</span></span>
  
<span data-ttu-id="1bf69-128">Dans une application d’API managée EWS, vous spécifiez le SID avec la valeur d’énumération [ConnectingIdType. sid](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1bf69-128">In an EWS Managed API application, you specify the SID along with the [ConnectingIdType.SID](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

<span data-ttu-id="1bf69-129">Dans une demande de SOAP EWS, l’élément [sid](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) contient le SID du compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1bf69-129">In an EWS SOAP request, the [SID](https://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) element contains the SID for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a><span data-ttu-id="1bf69-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1bf69-130">See also</span></span>


- [<span data-ttu-id="1bf69-131">Emprunt d'identité et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1bf69-131">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="1bf69-132">Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange</span><span class="sxs-lookup"><span data-stu-id="1bf69-132">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [<span data-ttu-id="1bf69-133">Classe de ExchangeService</span><span class="sxs-lookup"><span data-stu-id="1bf69-133">ExchangeService class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [<span data-ttu-id="1bf69-134">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1bf69-134">ExchangeImpersonation</span></span>](https://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

