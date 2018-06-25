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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754841"
---
# <a name="identify-the-account-to-impersonate"></a><span data-ttu-id="65bd0-103">Identifier le compte pour emprunter l’identité</span><span class="sxs-lookup"><span data-stu-id="65bd0-103">Identify the account to impersonate</span></span>

<span data-ttu-id="65bd0-104">Découvrez comment votre application de service utilise EWS pour identifier l’utilisateur pour emprunter l’identité.</span><span class="sxs-lookup"><span data-stu-id="65bd0-104">Learn how your service application uses EWS to identify the user to impersonate.</span></span>
  
<span data-ttu-id="65bd0-105">Votre application de service identifie le compte d’utilisateur pour emprunter l’identité à l’aide d’un des trois identificateurs suivants :</span><span class="sxs-lookup"><span data-stu-id="65bd0-105">Your service application identifies the user account to impersonate by using one of the following three identifiers:</span></span>
  
- <span data-ttu-id="65bd0-106">L’adresse SMTP principale.</span><span class="sxs-lookup"><span data-stu-id="65bd0-106">The primary SMTP address.</span></span>
    
- <span data-ttu-id="65bd0-107">Le nom principe d’utilisateur (UPN).</span><span class="sxs-lookup"><span data-stu-id="65bd0-107">The user principle name (UPN).</span></span>
    
- <span data-ttu-id="65bd0-108">L’identificateur de sécurité (SID).</span><span class="sxs-lookup"><span data-stu-id="65bd0-108">The security identifier (SID).</span></span>
    
<span data-ttu-id="65bd0-109">L’identificateur que vous utilisez dépend, bien sûr, les informations que votre application est disponible.</span><span class="sxs-lookup"><span data-stu-id="65bd0-109">The identifier that you use depends, of course, on the information that your application has available.</span></span>
  
## <a name="identifying-the-user-account-to-impersonate"></a><span data-ttu-id="65bd0-110">Identifier le compte d’utilisateur pour emprunter l’identité</span><span class="sxs-lookup"><span data-stu-id="65bd0-110">Identifying the user account to impersonate</span></span>

<span data-ttu-id="65bd0-111">Votre application peut utiliser les demandes SOAP EWS ou API managées pour identifier le compte d’utilisateur qui il emprunte l’identité.</span><span class="sxs-lookup"><span data-stu-id="65bd0-111">Your application can use either the EWS Managed API or EWS SOAP requests to identify the user account that it is impersonating.</span></span> <span data-ttu-id="65bd0-112">L’API managée EWS utilise la propriété [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) pour identifier l’emprunt d’identité utilisateur.</span><span class="sxs-lookup"><span data-stu-id="65bd0-112">The EWS Managed API uses the [ExchangeService.ImpersonatedUserId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.impersonateduserid.aspx) property to identify the impersonated user.</span></span> <span data-ttu-id="65bd0-113">EWS utilise l’élément [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) , comme illustré dans le fragment XML suivant.</span><span class="sxs-lookup"><span data-stu-id="65bd0-113">EWS uses the [ExchangeImpersonation](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx) element, as shown in the following XML fragment.</span></span> 
  
```XML
<soap:Header>
    <t:ExchangeImpersonation>
        <t:ConnectingSID>
            Identifier
        </t:ConnectingSID>
    </t:ExchangeImpersonation>
</soap:Header>
```

<span data-ttu-id="65bd0-114">Chacune des sections ci-dessous montre comment utiliser un des identificateurs.</span><span class="sxs-lookup"><span data-stu-id="65bd0-114">Each of the following sections shows how to use one of the identifiers.</span></span> <span data-ttu-id="65bd0-115">Pour obtenir un exemple qui illustre l’identificateur de l’emprunt d’identité en action, voir [Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange](how-to-add-appointments-by-using-exchange-impersonation.md).</span><span class="sxs-lookup"><span data-stu-id="65bd0-115">For an example that shows the impersonation identifier in action, see [Add appointments by using Exchange impersonation](how-to-add-appointments-by-using-exchange-impersonation.md).</span></span>
  
### <a name="use-the-smtp-email-address-to-identify-the-user-account"></a><span data-ttu-id="65bd0-116">Utiliser l’adresse de messagerie SMTP pour identifier le compte d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="65bd0-116">Use the SMTP email address to identify the user account</span></span>

<span data-ttu-id="65bd0-117">L’adresse de messagerie SMTP est l’adresse de messagerie principale qui est associé à un compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="65bd0-117">The SMTP email address is the primary email address that is associated with a user account.</span></span>
  
<span data-ttu-id="65bd0-118">Dans une application d’API managées, vous spécifiez l’adresse de messagerie SMTP ainsi que la valeur d’énumération [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="65bd0-118">In an EWS Managed API application, you specify the SMTP email address along with the [ConnectingIdType.SMTP](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SMTP, "alisa@contoso.com");
```

<span data-ttu-id="65bd0-119">Dans une demande SOAP EWS, l’élément [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) contient l’adresse de messagerie pour le compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="65bd0-119">In an EWS SOAP request, the [PrimarySmtpAddress](http://msdn.microsoft.com/library/eee79904-9412-4e61-b9b8-aff0ce25fade%28Office.15%29.aspx) element contains the email address for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrimarySmtpAddress>alisa@contoso.com</t: PrimarySmtpAddress>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-upn-to-identify-the-user-account"></a><span data-ttu-id="65bd0-120">L’UPN permet d’identifier le compte d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="65bd0-120">Use the UPN to identify the user account</span></span>

<span data-ttu-id="65bd0-121">L’UPN contient le nom de domaine complet (FQDN) pour l’emplacement du compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="65bd0-121">The UPN contains the fully qualified domain name (FQDN) for the location of the user account.</span></span> <span data-ttu-id="65bd0-122">Ce n’est pas nécessairement domaine de boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="65bd0-122">This is not necessarily the user's mailbox domain.</span></span> <span data-ttu-id="65bd0-123">L’attribut **UserPrincipleName** doit être correctement définie sur le compte d’utilisateur dans les Services de domaine Active Directory (AD DS) pour la recherche de l’utilisateur aboutisse.</span><span class="sxs-lookup"><span data-stu-id="65bd0-123">The **UserPrincipleName** attribute must be set correctly on the user account in Active Directory Domain Services (AD DS) for the user lookup to succeed.</span></span> 
  
<span data-ttu-id="65bd0-124">Dans une application d’API managées, vous spécifiez l’UPN ainsi que la valeur d’énumération [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="65bd0-124">In an EWS Managed API application, you specify the UPN along with the [ConnectingIdType.PrincipleName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.PrincipleName, "alias@billing.contoso.com");
```

<span data-ttu-id="65bd0-125">Dans une demande SOAP EWS, le [au PrincipalName, élément (ConnectingSIDType, complexType) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx) élément contient l’UPN du compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="65bd0-125">In an EWS SOAP request, the [PrincipalName element (ConnectingSIDType complexType) (EWS)](http://msdn.microsoft.com/library/6aac5388-c971-817b-b0bb-095a2639c6de%28Office.15%29.aspx) element contains the UPN for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:PrincipalName>alisa@billing.contoso.com</t:PrincipalName>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

### <a name="use-the-sid-to-identify-the-user-account"></a><span data-ttu-id="65bd0-126">Utiliser le SID pour identifier le compte d’utilisateur</span><span class="sxs-lookup"><span data-stu-id="65bd0-126">Use the SID to identify the user account</span></span>

<span data-ttu-id="65bd0-127">Le SID est l’identificateur du compte pour être représenté dans le formulaire de sécurité descripteur definition language (SDDL).</span><span class="sxs-lookup"><span data-stu-id="65bd0-127">The SID is the identifier of the account to be impersonated in security descriptor definition language (SDDL) form.</span></span>
  
<span data-ttu-id="65bd0-128">Dans une application API managée EWS, vous spécifiez le SID ainsi que la valeur d’énumération [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) .</span><span class="sxs-lookup"><span data-stu-id="65bd0-128">In an EWS Managed API application, you specify the SID along with the [ConnectingIdType.SID](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.connectingidtype.aspx) enumeration value.</span></span> 
  
```cs
exchangeServiceInstance.ImpersonatedUserId = new ImpersonatedUserId(ConnectingIdType.SID, "S-1-5-21-1493619105-1843311271-3936346804-1118");
```

<span data-ttu-id="65bd0-129">Dans une demande SOAP EWS, l’élément [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) contient l’identificateur de sécurité pour le compte d’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="65bd0-129">In an EWS SOAP request, the [SID](http://msdn.microsoft.com/library/2f33b29b-163b-4106-a74d-6fb76ec38951%28Office.15%29.aspx) element contains the SID for the user account.</span></span> 
  
```XML
<soap:Header>
  <t:ExchangeImpersonation>
    <t:ConnectingSID>
      <t:SID>S-1-5-21-1493619105-1843311271-3936346804-1118</t:SID>
    </t:ConnectingSID>
  </t:ExchangeImpersonation>
</soap:Header>
```

## <a name="see-also"></a><span data-ttu-id="65bd0-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="65bd0-130">See also</span></span>


- [<span data-ttu-id="65bd0-131">Emprunt d'identité et EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="65bd0-131">Impersonation and EWS in Exchange</span></span>](impersonation-and-ews-in-exchange.md)
    
- [<span data-ttu-id="65bd0-132">Ajouter des rendez-vous à l’aide de l’emprunt d’identité Exchange</span><span class="sxs-lookup"><span data-stu-id="65bd0-132">Add appointments by using Exchange impersonation</span></span>](how-to-add-appointments-by-using-exchange-impersonation.md)
    
- [<span data-ttu-id="65bd0-133">Classe de ExchangeService</span><span class="sxs-lookup"><span data-stu-id="65bd0-133">ExchangeService class</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.aspx)
    
- [<span data-ttu-id="65bd0-134">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="65bd0-134">ExchangeImpersonation</span></span>](http://msdn.microsoft.com/library/d8cbac49-47d0-4745-a2a7-545d33f8da93%28Office.15%29.aspx)
    

