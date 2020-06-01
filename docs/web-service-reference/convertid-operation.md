---
title: Opération ConvertId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConvertId
api_type:
- schema
ms.assetid: 47d96cf6-9e2f-4fc0-9682-7258d3fbf918
description: Trouvez des informations sur l’opération EWS ConvertId.
ms.openlocfilehash: 36bd47d3fc7c7ca7cea7b38222abb25fba6074ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44452551"
---
# <a name="convertid-operation"></a><span data-ttu-id="6af8c-103">Opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="6af8c-103">ConvertId operation</span></span>

<span data-ttu-id="6af8c-104">Trouvez des informations sur l’opération EWS **ConvertId** .</span><span class="sxs-lookup"><span data-stu-id="6af8c-104">Find information about the **ConvertId** EWS operation.</span></span> 
  
<span data-ttu-id="6af8c-105">L’opération EWS (Exchange Web Services) **ConvertId** convertit les identificateurs d’élément et de dossier entre les formats acceptés par Exchange Online, Exchange Online dans le cadre d’Office 365 et les versions locales d’Exchange à partir d’exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6af8c-105">The **ConvertId** Exchange Web Services (EWS) operation converts item and folder identifiers between formats that are accepted by Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with Exchange Server 2013.</span></span> 
  
## <a name="using-the-convertid-operation"></a><span data-ttu-id="6af8c-106">Utilisation de l’opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="6af8c-106">Using the ConvertId operation</span></span>
<span data-ttu-id="6af8c-107"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="6af8c-107"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="6af8c-108">Vous pouvez convertir les identificateurs suivants à l’aide de l’opération **ConvertId** :</span><span class="sxs-lookup"><span data-stu-id="6af8c-108">You can convert the following identifiers by using the **ConvertId** operation:</span></span> 
  
- <span data-ttu-id="6af8c-109">Format d’identificateur pour EWS dans la version initiale d’Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="6af8c-109">The identifier format for EWS in the initial release version of Exchange 2007.</span></span> <span data-ttu-id="6af8c-110">Cette valeur est représentée par la `EwsLegacyId` valeur d’énumération dans l’énumération [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6af8c-110">This is represented by the  `EwsLegacyId` enumeration value in the [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="6af8c-111">Format d’identificateur pour EWS dans Exchange 2007 SP1 ou Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="6af8c-111">The identifier format for EWS in Exchange 2007 SP1 or Exchange 2010.</span></span> <span data-ttu-id="6af8c-112">Cette valeur est représentée par la `EwsId` valeur d’énumération dans [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6af8c-112">This is represented by the  `EwsId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="6af8c-113">Identificateur MAPI, comme dans la propriété **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="6af8c-113">The MAPI identifier, as in the **PR_ENTRYID** property.</span></span> <span data-ttu-id="6af8c-114">Cette valeur est représentée par la `EntryId` valeur d’énumération dans l’énumération [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="6af8c-114">This is represented by the  `EntryId` enumeration value in the [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx) enumeration.</span></span> 
    
- <span data-ttu-id="6af8c-115">Identificateur d’événement de calendrier de disponibilité.</span><span class="sxs-lookup"><span data-stu-id="6af8c-115">The availability calendar event identifier.</span></span> <span data-ttu-id="6af8c-116">Il s’agit d’une représentation codée en hexadécimal de la propriété **PR_ENTRYID** .</span><span class="sxs-lookup"><span data-stu-id="6af8c-116">This is a hexadecimal-encoded representation of the **PR_ENTRYID** property.</span></span> <span data-ttu-id="6af8c-117">Cette valeur est représentée par la `HexEntryId` valeur d’énumération dans [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6af8c-117">This is represented by the  `HexEntryId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span>
    
- <span data-ttu-id="6af8c-118">Identificateur de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="6af8c-118">The Exchange store identifier.</span></span> <span data-ttu-id="6af8c-119">Cette valeur est représentée par la `StoreId` valeur d’énumération dans [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="6af8c-119">This is represented by the  `StoreId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="6af8c-120">L’opération **ConvertId** ne convertit pas les identificateurs de dossiers publics de l’identificateur EWS en identificateur de magasin.</span><span class="sxs-lookup"><span data-stu-id="6af8c-120">The **ConvertId** operation does not convert public folder identifiers from the EWS identifier to the store identifier.</span></span> 
    
- <span data-ttu-id="6af8c-121">Identificateur d’Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6af8c-121">The Outlook Web App identifier.</span></span> <span data-ttu-id="6af8c-122">Cette valeur est représentée par la `OwaId` valeur d’énumération dans [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="6af8c-122">This is represented by the  `OwaId` enumeration value in [IdFormat](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.idformat%28v=exchg.80%29.aspx)</span></span>
    
    <span data-ttu-id="6af8c-123">La transmission des URL créées à partir de cet identificateur vers Outlook Web App n’est pas prise en charge.</span><span class="sxs-lookup"><span data-stu-id="6af8c-123">The passing of URLs that are created from this identifier to Outlook Web App is not supported.</span></span> <span data-ttu-id="6af8c-124">L’identificateur d’Outlook Web App est applicable à Exchange 2007 et Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="6af8c-124">The Outlook Web App identifier is applicable to Exchange 2007 and Exchange 2010.</span></span> <span data-ttu-id="6af8c-125">Outlook Web App pour Exchange Online et les versions d’Exchange commençant par Exchange Server 2013 utilisent des identificateurs EWS.</span><span class="sxs-lookup"><span data-stu-id="6af8c-125">Outlook Web App for Exchange Online and versions of Exchange starting with Exchange Server 2013 uses EWS identifiers.</span></span>
    
<span data-ttu-id="6af8c-126">L’opération **ConvertId** ne fonctionne pas comme prévu lors de la conversion d’identificateurs de dossiers publics de l’identificateur EWS en identificateur de magasin dans Exchange Online et Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="6af8c-126">The **ConvertId** operation does not work as expected when converting public folder identifiers from the EWS identifier to the store identifier in Exchange Online and Exchange 2013.</span></span> <span data-ttu-id="6af8c-127">Vous pouvez mettre à jour manuellement l’identificateur renvoyé sous forme de solution de contournement.</span><span class="sxs-lookup"><span data-stu-id="6af8c-127">You can manually update the identifier that is returned as a workaround.</span></span> <span data-ttu-id="6af8c-128">Pour mettre à jour manuellement l’identificateur :</span><span class="sxs-lookup"><span data-stu-id="6af8c-128">To manually update the identifier:</span></span> 
  
1. <span data-ttu-id="6af8c-129">Dans le code de votre application, déterminez si l’élément/dossier cible se trouve dans un dossier public.</span><span class="sxs-lookup"><span data-stu-id="6af8c-129">In your application code, determine whether the target item/folder is in a public folder.</span></span> 
    
2. <span data-ttu-id="6af8c-130">Décodez la chaîne d’identificateur codée en base64.</span><span class="sxs-lookup"><span data-stu-id="6af8c-130">Decode the Base64-encoded identifier string.</span></span>
    
3. <span data-ttu-id="6af8c-131">Vérifiez que le type Byte (21ème octet) a la valeur 7.</span><span class="sxs-lookup"><span data-stu-id="6af8c-131">Verify that the type byte (21st byte) has a value of 7.</span></span> <span data-ttu-id="6af8c-132">Une valeur de 7 indique que l’identificateur est dans un format incorrect.</span><span class="sxs-lookup"><span data-stu-id="6af8c-132">A value of 7 indicates that the identifier is in the incorrect format.</span></span>
    
4. <span data-ttu-id="6af8c-133">Ignorez les quatre premiers octets.</span><span class="sxs-lookup"><span data-stu-id="6af8c-133">Skip the first four bytes.</span></span> <span data-ttu-id="6af8c-134">Elles doivent être définies sur zéro.</span><span class="sxs-lookup"><span data-stu-id="6af8c-134">They must be set to zero.</span></span>
    
5. <span data-ttu-id="6af8c-135">Mettez à jour les 16 octets suivants avec le GUID suivant : 1A447390AA6611CD9BC800AA002FC45A</span><span class="sxs-lookup"><span data-stu-id="6af8c-135">Update the next 16 bytes with the following GUID: 1A447390AA6611CD9BC800AA002FC45A</span></span>
    
6. <span data-ttu-id="6af8c-136">Mettez à jour l’octet suivant (type Byte) avec une valeur de 9.</span><span class="sxs-lookup"><span data-stu-id="6af8c-136">Update the next byte (type byte) with a value of 9.</span></span>
    
7. <span data-ttu-id="6af8c-137">Remplacez l’identificateur par une chaîne codée en base 64.</span><span class="sxs-lookup"><span data-stu-id="6af8c-137">Change the identifier to a Base64-encoded string.</span></span>
    
> [!NOTE]
> <span data-ttu-id="6af8c-138">L’opération **ConvertId** vérifie qu’une adresse SMTP donnée a un format valide.</span><span class="sxs-lookup"><span data-stu-id="6af8c-138">The **ConvertId** operation validates that a given SMTP address has a valid format.</span></span> <span data-ttu-id="6af8c-139">L’opération ne détermine pas si une adresse SMTP représente une boîte aux lettres valide.</span><span class="sxs-lookup"><span data-stu-id="6af8c-139">The operation does not determine whether an SMTP address represents a valid mailbox.</span></span> 
  
<span data-ttu-id="6af8c-140">L’opération **ConvertId** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="6af8c-140">The **ConvertId** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="6af8c-141">**Tableau 1. En-têtes SOAP d’opération ConvertId**</span><span class="sxs-lookup"><span data-stu-id="6af8c-141">**Table 1. ConvertId operation SOAP headers**</span></span>

|<span data-ttu-id="6af8c-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="6af8c-142">**Header**</span></span>|<span data-ttu-id="6af8c-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6af8c-143">**Element**</span></span>|<span data-ttu-id="6af8c-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="6af8c-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6af8c-145">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="6af8c-145">Impersonation</span></span>  <br/> |[<span data-ttu-id="6af8c-146">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="6af8c-146">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="6af8c-147">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="6af8c-147">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="6af8c-148">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="6af8c-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6af8c-149">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="6af8c-149">RequestVersion</span></span>  <br/> |[<span data-ttu-id="6af8c-150">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="6af8c-150">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="6af8c-151">Identifie la version de schéma de la demande d’opération applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="6af8c-151">Identifies the schema version for the operation request This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6af8c-152">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="6af8c-152">ServerVersion</span></span>  <br/> |[<span data-ttu-id="6af8c-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="6af8c-153">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6af8c-154">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="6af8c-154">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="6af8c-155">Ceci s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="6af8c-155">This is applicable to a response.</span></span>  <br/> |
   
## <a name="convertid-operation-request-example"></a><span data-ttu-id="6af8c-156">Exemple de requête d’opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="6af8c-156">ConvertId operation request example</span></span>
<span data-ttu-id="6af8c-157"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="6af8c-157"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="6af8c-158">L’exemple de requête **ConvertId** suivant montre comment convertir un identificateur EWS en identificateur d’Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6af8c-158">The following example of a **ConvertId** request shows how to convert from an EWS identifier to an Outlook Web App identifier.</span></span> 
  
<span data-ttu-id="6af8c-159">L’élément [RequestServerVersion](requestserverversion.md) de l’en-tête SOAP doit être défini sur Exchange2007_SP1 ou une version ultérieure pour que cette opération fonctionne.</span><span class="sxs-lookup"><span data-stu-id="6af8c-159">The [RequestServerVersion](requestserverversion.md) element in the SOAP header must be set to Exchange2007_SP1 or later for this operation to work.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6af8c-160">Identificateur de l'élément a été raccourcie afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="6af8c-160">The item identifier has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <ConvertId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               DestinationFormat="OwaId">
      <SourceIds>
        <t:AlternateId Format="EwsId" Id="AAMkAGZhN2IxYTA0LWNiNzItN="
                       Mailbox="user1@example.com"/>
      </SourceIds>
    </ConvertId>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-response-example"></a><span data-ttu-id="6af8c-161">Exemple de réponse d’opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="6af8c-161">ConvertId operation response example</span></span>
<span data-ttu-id="6af8c-162"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="6af8c-162"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="6af8c-163">L’exemple suivant montre une réponse réussie à une demande **ConvertId** .</span><span class="sxs-lookup"><span data-stu-id="6af8c-163">The following example shows a successful response to a **ConvertId** request.</span></span> <span data-ttu-id="6af8c-164">Cet exemple de réponse contient un identificateur Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="6af8c-164">This response example contains an Outlook Web App identifier.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6af8c-165">L’identificateur d’Outlook Web App a été raccourci pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="6af8c-165">The Outlook Web App identifier has been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                         MajorBuildNumber="191" MinorBuildNumber="0" 
                         Version="Exchange2010" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <AlternateId xsi:type="t:AlternateIdType" Format="OwaId" Id="RgAAAAAS2%2" 
                         Mailbox="user@example.com" />
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="convertid-operation-error-response-example"></a><span data-ttu-id="6af8c-166">Exemple de réponse d’erreur d’opération ConvertId</span><span class="sxs-lookup"><span data-stu-id="6af8c-166">ConvertId operation error response example</span></span>
<span data-ttu-id="6af8c-167"><a name="bk_usingConvertId"> </a></span><span class="sxs-lookup"><span data-stu-id="6af8c-167"><a name="bk_usingConvertId"> </a></span></span>

<span data-ttu-id="6af8c-168">L’exemple suivant montre la réponse à une demande contenant un type de format d’identificateur incorrect.</span><span class="sxs-lookup"><span data-stu-id="6af8c-168">The following example shows the response to a request that contains the wrong type of identifier format.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <ServerVersionInfo MajorVersion="8" MinorVersion="1" 
                       MajorBuildNumber="206" MinorBuildNumber="0"
                       Version="Exchange2010" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ConvertIdResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <ConvertIdResponseMessage ResponseClass="Error">
          <MessageText>Id is malformed.</MessageText>
          <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
          <DescriptiveLinkKey>0</DescriptiveLinkKey>
        </ConvertIdResponseMessage>
      </ResponseMessages>
    </ConvertIdResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="version-differences"></a><span data-ttu-id="6af8c-169">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="6af8c-169">Version differences</span></span>
<span data-ttu-id="6af8c-170"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="6af8c-170"><a name="bk_ConvertIdVersionDiff"> </a></span></span>

<span data-ttu-id="6af8c-171">Le format d’identificateur EWS a changé entre la version initiale d’Exchange 2007 et Exchange 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6af8c-171">The EWS identifier format changed between the initial release version of Exchange 2007 and Exchange 2007 Service Pack 1 (SP1).</span></span> <span data-ttu-id="6af8c-172">Exchange Online dans le cadre d’Office 365, Exchange Online et les versions locales d’Exchange à partir d’Exchange 2010 utilisent le même format d’identificateur que celui utilisé par Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="6af8c-172">Exchange Online as part of Office 365, Exchange Online, and on-premises versions of Exchange starting with Exchange 2010 use the same identifier format that Exchange 2007 SP1 uses.</span></span>
  
<span data-ttu-id="6af8c-173">L’opération **ConvertId** convertit des identificateurs de dossiers publics de l’identificateur EWS en identificateur de magasin dans Exchange 2007 et Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="6af8c-173">The **ConvertId** operation converts public folder identifiers from the EWS identifier to the store identifier in Exchange 2007 and Exchange 2010.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6af8c-174">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6af8c-174">See also</span></span>
<span data-ttu-id="6af8c-175"><a name="bk_ConvertIdVersionDiff"> </a></span><span class="sxs-lookup"><span data-stu-id="6af8c-175"><a name="bk_ConvertIdVersionDiff"> </a></span></span>

- [<span data-ttu-id="6af8c-176">Conversion des identificateurs</span><span class="sxs-lookup"><span data-stu-id="6af8c-176">Converting Identifiers</span></span>](https://msdn.microsoft.com/library/a5391746-b6ef-4f48-8fc8-8255258651aa%28Office.15%29.aspx)
    
- [<span data-ttu-id="6af8c-177">ConvertIdType</span><span class="sxs-lookup"><span data-stu-id="6af8c-177">ConvertIdType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ConvertIdType.aspx)
    
- [<span data-ttu-id="6af8c-178">ConvertId</span><span class="sxs-lookup"><span data-stu-id="6af8c-178">ConvertId</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ExchangeServiceBinding.ConvertId.aspx)
    

