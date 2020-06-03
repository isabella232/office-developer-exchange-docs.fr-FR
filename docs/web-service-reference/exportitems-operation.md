---
title: Opération ExportItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItems
api_type:
- schema
ms.assetid: e2846abb-0b16-4732-bbd8-038a674672f6
description: L’opération ExportItems exporte les éléments hors d’une boîte aux lettres.
ms.openlocfilehash: 547a490a27d2414d2eda1d89cdac036a34eddccd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526045"
---
# <a name="exportitems-operation"></a><span data-ttu-id="959e6-103">Opération ExportItems</span><span class="sxs-lookup"><span data-stu-id="959e6-103">ExportItems operation</span></span>

<span data-ttu-id="959e6-104">L’opération **ExportItems** exporte les éléments hors d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="959e6-104">The **ExportItems** operation exports items out of a mailbox.</span></span> 
  
## <a name="exportitems-request-example"></a><span data-ttu-id="959e6-105">Exemple de requête ExportItems</span><span class="sxs-lookup"><span data-stu-id="959e6-105">ExportItems request example</span></span>

### <a name="description"></a><span data-ttu-id="959e6-106">Description</span><span class="sxs-lookup"><span data-stu-id="959e6-106">Description</span></span>

<span data-ttu-id="959e6-107">L’exemple de requête **ExportItems** suivant montre comment créer une demande pour obtenir trois éléments exportés à partir d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="959e6-107">The following example of an **ExportItems** request shows how to form a request to get three items exported from a mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="959e6-108">Code</span><span class="sxs-lookup"><span data-stu-id="959e6-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExportItems>
      <m:ItemIds>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA="/>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89FAAA="/>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY87NAAA="/>
      </m:ItemIds>
    </m:ExportItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="959e6-109">Commentaire</span><span class="sxs-lookup"><span data-stu-id="959e6-109">Comment</span></span>

<span data-ttu-id="959e6-110">Les identificateurs d’élément de l’exemple ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="959e6-110">The item identifiers in the example have been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="959e6-111">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="959e6-111">Request elements</span></span>

<span data-ttu-id="959e6-112">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="959e6-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="959e6-113">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="959e6-113">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="959e6-114">ExportItems</span><span class="sxs-lookup"><span data-stu-id="959e6-114">ExportItems</span></span>](exportitems.md)
    
- [<span data-ttu-id="959e6-115">ItemIds (NonEmptyArrayOfItemIdsType)</span><span class="sxs-lookup"><span data-stu-id="959e6-115">ItemIds (NonEmptyArrayOfItemIdsType)</span></span>](itemids-nonemptyarrayofitemidstype.md)
    
- [<span data-ttu-id="959e6-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="959e6-116">ItemId</span></span>](itemid.md)
    
## <a name="successful-exportitems-response-example"></a><span data-ttu-id="959e6-117">Exemple de réponse ExportItems réussi</span><span class="sxs-lookup"><span data-stu-id="959e6-117">Successful ExportItems response example</span></span>

### <a name="description"></a><span data-ttu-id="959e6-118">Description</span><span class="sxs-lookup"><span data-stu-id="959e6-118">Description</span></span>

<span data-ttu-id="959e6-119">L’exemple suivant montre une réponse réussie à une demande **ExportItems** .</span><span class="sxs-lookup"><span data-stu-id="959e6-119">The following example shows a successful response to an **ExportItems** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="959e6-120">Code</span><span class="sxs-lookup"><span data-stu-id="959e6-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <t:ServerVersionInfo MajorVersion="14"
    MinorVersion="1"
    MajorBuildNumber="139"
    MinorBuildNumber="0"
    Version="Exchange2010_SP1"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
    xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ExportItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA=" ChangeKey="FwAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
            YwBvAG0AAABTAE0AVABQAAAAVQBzAGUAcgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUA
            eAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMAbwBmAHQALgBjAG8AbQAAALCE/jlMAAAAVQBzAGUA
            cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
            bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
          </m:Data>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89FAAA=" ChangeKey="FwAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAAAAAEYAJACA
            QAAyAAAh9SpR08oBAwAEQAMAFkANABMOAwAAQAMAIQ4AAAAAsIQSN0oAAAAyAGEAYgAxADYA
            MQA2ADYALQBhAGUANQBkAC0ANAAyAGUAZgAtAGEANQA1ADkALQBjADgAOQAwADgANwBkADIA
            MwBkADgANAAAAAMACzf/////AwAgDmQEAAADAPcPAAAAAEAABzBPMXstUdPKAUAACDBPMXst
            UdPKAQMABTcFAAAAsIQONx4AAABtAGUAcwBzAGEAZwBlAC8AcgBmAGMAOAAyADIAAACwhAEw
            IgAAAE0AbwBzAHQAIABmAGEAcwBjAGkAbgBhAHQAaQBuAGcAAAACAfkPBAAAAAAAAAADAAFA
            FABKZ3QrAAAAZF2mAwAXAAEAAACwhBoAEgAAAEkAUABNAC4ATgBvAHQAZQAAAAMANgAAAAAA
            sIQ3ACIAAABNAG8AcwB0ACAAZgBhAHMAYwBpAG4AYQB0AGkAbgBnAAAAQAA5AACq+za80coB
            AgE7AGUAAABFWDovTz1GSVJTVCBPUkdBTklaQVRJT04vT1U9RVhDSEFOR0UgQURNSU5JU1RS
            QVRJVkUgR1JPVVAgKEZZRElCT0hGMjNTUERMVCkvQ049UkVDSVBJRU5UUy9DTj1VU0VST05F
            ALCEPQACAAAAAAACAUEAfgAAAAAAAADcp0DIwEIQGrS5CAArL+GCAQAAAAAAAAAvTz1GSVJT
            VCBPUkdBTklaQVRJT04vT1U9RVhDSEFOR0UgQURNSU5JU1RSQVRJVkUgR1JPVVAgKEZZRElC
            T0hGMjNTUERMVCkvQ049UkVDSVBJRU5UUy9DTj1VU0VST05FALCEQgAQAAAAVQB
          </m:Data>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY87NAAA=" ChangeKey="CQAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAAAAAEYAJACA
            BAAAAAYAAAABDouAAAACAAAAEiAAAOSECEBbAAAAL089RklSU1QgT1JHQU5JWkFUSU9OL09V
            PUVYQ0hBTkdFIEFETUlOSVNUUkFUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJF
            Q0lQSUVOVFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAAALACMAAAAL
            ACkAAAADADYAAAAAALCENwAyAAAASQBuAHQAZQByAGUAcwB0AGkAbgBnACAALQAgAGYAcgBv
            AG0AIABFAFcAUwBNAEEAAABAADkAAHZeFxfRygECATsAZQAAAEVYOi9PPUZJUlNUIE9SR0FO
            SVpBVElPTi9PVT1FWENIQU5HRSBBRE1JTklTVFJBVElWRSBHUk9VUCAoRllESUJPSEYyM1NQ
            RExUKS9DTj1SRUNJUElFTlRTL0NOPVVTRVJPTkUAsIQ9AAIAAAAAAAIBPwB+AAAAAAAAANyn
            QMjAQhAatLkIACsv4YIBAAAAAAAAAC9PPUZJUlNUIE9SR0FOSVpBVElPTi9PVT1FWENIQU5H
          </m:Data>
        </m:ExportItemsResponseMessage>
      </m:ResponseMessages>
    </m:ExportItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="comment"></a><span data-ttu-id="959e6-121">Commentaire</span><span class="sxs-lookup"><span data-stu-id="959e6-121">Comment</span></span>

<span data-ttu-id="959e6-122">Les identificateurs d’élément et les clés de modification de l’exemple ont été raccourcis pour conserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="959e6-122">The item identifiers and change keys in the example have been shortened to preserve readability.</span></span>
  
### <a name="response-elements"></a><span data-ttu-id="959e6-123">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="959e6-123">Response elements</span></span>

<span data-ttu-id="959e6-124">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="959e6-124">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="959e6-125">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="959e6-125">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="959e6-126">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="959e6-126">ExportItemsResponse</span></span>](exportitemsresponse.md)
    
- [<span data-ttu-id="959e6-127">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="959e6-127">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="959e6-128">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="959e6-128">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
    
- [<span data-ttu-id="959e6-129">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="959e6-129">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="959e6-130">ItemId</span><span class="sxs-lookup"><span data-stu-id="959e6-130">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="959e6-131">Données (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="959e6-131">Data (base64Binary)</span></span>](data-base64binary.md)
    
## <a name="exportitems-error-response-example"></a><span data-ttu-id="959e6-132">Exemple de réponse d’erreur ExportItems</span><span class="sxs-lookup"><span data-stu-id="959e6-132">ExportItems Error response example</span></span>

### <a name="description"></a><span data-ttu-id="959e6-133">Description</span><span class="sxs-lookup"><span data-stu-id="959e6-133">Description</span></span>

<span data-ttu-id="959e6-134">L’exemple suivant montre une réponse à la requête **ExportItems** qui contient deux erreurs et un élément exporté avec succès.</span><span class="sxs-lookup"><span data-stu-id="959e6-134">The following example shows a response to the **ExportItems** request that contains two errors and one successfully exported item.</span></span> <span data-ttu-id="959e6-135">Le premier élément de l’exemple est correctement exporté.</span><span class="sxs-lookup"><span data-stu-id="959e6-135">The first item in the example is successfully exported.</span></span> <span data-ttu-id="959e6-136">Le deuxième élément contient une clé de modification incorrecte.</span><span class="sxs-lookup"><span data-stu-id="959e6-136">The second item contains an incorrect change key.</span></span> <span data-ttu-id="959e6-137">Le troisième élément représente une tentative d’exportation d’un élément à partir d’une boîte aux lettres incorrecte.</span><span class="sxs-lookup"><span data-stu-id="959e6-137">The third item represents an attempt to export an item from the wrong mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="959e6-138">Code</span><span class="sxs-lookup"><span data-stu-id="959e6-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ExportItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ExportItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhOGU0oMf0GPIQeAAAAUC8iAABseAAAAUFZ7AAA=" ChangeKey="CQAAAA=="/>
          <m:Data>
            AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
            YwBvAG0AAABTAE0AVABQAAAAVQBzAGUAcgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUA
            eAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMAbwBmAHQALgBjAG8AbQAAALCE/jlMAAAAVQBzAGUA
            cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
            bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
          </m:Data>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The change key is invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidChangeKey</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExportItemsResponseMessage>
        <m:ExportItemsResponseMessage ResponseClass="Error">
          <m:MessageText>No mailbox with such guid.</m:MessageText>
          <m:ResponseCode>ErrorNonExistentMailbox</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:Value Name="MailboxGuid">f3f6f699-2254-40ce-9994-388d9d98419e</t:Value>
          </m:MessageXml>
        </m:ExportItemsResponseMessage>
      </m:ResponseMessages>
    </m:ExportItemsResponse>
  </s:Body>
</s:Envelope>

```

### <a name="comments"></a><span data-ttu-id="959e6-139">Commentaires</span><span class="sxs-lookup"><span data-stu-id="959e6-139">Comments</span></span>

<span data-ttu-id="959e6-140">Les identificateurs d’élément, les clés de modification et les données de l’exemple ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="959e6-140">The item identifiers, change keys, and data in the example have been shortened to preserve readability.</span></span>
  
### <a name="error-response-elements"></a><span data-ttu-id="959e6-141">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="959e6-141">Error response elements</span></span>

<span data-ttu-id="959e6-142">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="959e6-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="959e6-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="959e6-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="959e6-144">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="959e6-144">ExportItemsResponse</span></span>](exportitemsresponse.md)
    
- [<span data-ttu-id="959e6-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="959e6-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="959e6-146">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="959e6-146">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
    
- [<span data-ttu-id="959e6-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="959e6-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="959e6-148">ItemId</span><span class="sxs-lookup"><span data-stu-id="959e6-148">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="959e6-149">Données (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="959e6-149">Data (base64Binary)</span></span>](data-base64binary.md)
    
- [<span data-ttu-id="959e6-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="959e6-150">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="959e6-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="959e6-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="959e6-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="959e6-152">MessageXml</span></span>](messagexml.md)
    
- <span data-ttu-id="959e6-153">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="959e6-153">**Value**</span></span>
    
> [!NOTE]
> <span data-ttu-id="959e6-154">L’élément **value** n’existe pas dans le schéma.</span><span class="sxs-lookup"><span data-stu-id="959e6-154">The **Value** element does not exist in the schema.</span></span> <span data-ttu-id="959e6-155">Cet élément est valide car l’élément [messagexml](messagexml.md) , dans lequel l’élément instance de la **valeur** se produit, peut contenir n’importe quel code XML bien formé.</span><span class="sxs-lookup"><span data-stu-id="959e6-155">This element is valid because the [MessageXml](messagexml.md) element, in which the **Value** instance element occurs, can contain any well-formed XML.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="959e6-156">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="959e6-156">See also</span></span>



[<span data-ttu-id="959e6-157">Opération UploadItems</span><span class="sxs-lookup"><span data-stu-id="959e6-157">UploadItems operation</span></span>](uploaditems-operation.md)


[<span data-ttu-id="959e6-158">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="959e6-158">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="959e6-159">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="959e6-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

