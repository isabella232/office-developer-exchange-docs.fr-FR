---
title: Acheminer les demandes de contenu de dossier public
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: Toutes les demandes d’informations de dossier public qui impliquent le contenu du dossier public doivent être acheminées vers la boîte aux lettres de dossiers publics qui contient le contenu du dossier cible. Pour acheminer les demandes vers cette boîte aux lettres, vous devez définir les en-têtes X-AnchorMailbox et X-PublicFolderMailbox sur des valeurs spécifiques.
ms.openlocfilehash: 523b9c8efc65253f7970fffeb5800e451784522d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527743"
---
# <a name="route-public-folder-content-requests"></a><span data-ttu-id="4aead-104">Acheminer les demandes de contenu de dossier public</span><span class="sxs-lookup"><span data-stu-id="4aead-104">Route public folder content requests</span></span>

<span data-ttu-id="4aead-105">Toutes les demandes d’informations de dossier public qui impliquent le contenu du dossier public doivent être acheminées vers la boîte aux lettres de dossiers publics qui contient le contenu du dossier cible.</span><span class="sxs-lookup"><span data-stu-id="4aead-105">All requests for public folder information that involve the content of the public folder need to be routed to the public folder mailbox that holds the content for the target folder.</span></span> <span data-ttu-id="4aead-106">Pour acheminer les demandes vers cette boîte aux lettres, vous devez définir les en-têtes **x-AnchorMailbox** et **x-PublicFolderMailbox** sur des valeurs spécifiques.</span><span class="sxs-lookup"><span data-stu-id="4aead-106">To route the requests to that mailbox, you need to set the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers to specific values.</span></span> 
  
<span data-ttu-id="4aead-107">Le tableau suivant fournit une vue d’ensemble du processus :</span><span class="sxs-lookup"><span data-stu-id="4aead-107">The following table provides an overview of the process:</span></span>
  
<span data-ttu-id="4aead-108">**Vue d’ensemble des dossiers publics**</span><span class="sxs-lookup"><span data-stu-id="4aead-108">**Public folder overview**</span></span>

|<span data-ttu-id="4aead-109">En-tête</span><span class="sxs-lookup"><span data-stu-id="4aead-109">Header</span></span>|<span data-ttu-id="4aead-110">De quoi ai-je besoin ?</span><span class="sxs-lookup"><span data-stu-id="4aead-110">What do I need?</span></span>|<span data-ttu-id="4aead-111">Comment puis-je l’obtenir ?</span><span class="sxs-lookup"><span data-stu-id="4aead-111">How do I get it?</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4aead-112">**X-AnchorMailbox**</span><span class="sxs-lookup"><span data-stu-id="4aead-112">**X-AnchorMailbox**</span></span> <br/> |<span data-ttu-id="4aead-113">1. [les valeurs x-AnchorMailbox et x-PublicFolderInformation](how-to-route-public-folder-hierarchy-requests.md) pour la boîte aux lettres de la hiérarchie de dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="4aead-113">1. [The X-AnchorMailbox and X-PublicFolderInformation values ](how-to-route-public-folder-hierarchy-requests.md) for the public folder hierarchy mailbox.</span></span><br/><br/><span data-ttu-id="4aead-114">2. le GUID de la boîte aux lettres de dossiers publics qui contient le contenu de la boîte aux lettres, qui est envoyé au service de découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="4aead-114">2. The GUID of the public folder mailbox that contains the mailbox content, which is sent to the Autodiscover service.</span></span><br/><br/>  <span data-ttu-id="4aead-115">La **AutoDiscoverSMTPAddress** dans la réponse découverte automatique devient la valeur de l’en-tête **X-AnchorMailbox** .</span><span class="sxs-lookup"><span data-stu-id="4aead-115">The **AutoDiscoverSMTPAddress** in the Autodisover response becomes the value of the **X-AnchorMailbox** header.</span></span>  <br/> <span data-ttu-id="4aead-116">![TODO](media/Ex15_PF_PFContent.png)</span><span class="sxs-lookup"><span data-stu-id="4aead-116">![TODO](media/Ex15_PF_PFContent.png)</span></span>| <span data-ttu-id="4aead-117">1. Utilisez l’exemple de code de cet article, qui [implémente l’API managée EWS](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="4aead-117">1. Use the code example in this article, which [implements the EWS Managed API](#bk_determineguidewsma).</span></span> <span data-ttu-id="4aead-118">Vous pouvez [utiliser EWS](#bk_determineguidews) et convertir vos résultats pour obtenir un GUID.</span><span class="sxs-lookup"><span data-stu-id="4aead-118">Or [use EWS](#bk_determineguidews) and convert your results to obtain a GUID.</span></span><br/><br/><span data-ttu-id="4aead-119">2. [effectuez une demande de découverte automatique](#bk_makeautodrequest) à l’aide du GUID plus le nom de domaine.</span><span class="sxs-lookup"><span data-stu-id="4aead-119">2. [Make an Autodiscover request](#bk_makeautodrequest) by using the GUID plus the domain name.</span></span><br/><br/><span data-ttu-id="4aead-120">3. Utilisez la valeur de l’élément **AutoDiscoverSMTPAddress** renvoyée dans la réponse de découverte automatique pour [renseigner la valeur des en-têtes](#bk_setheadervalues).</span><span class="sxs-lookup"><span data-stu-id="4aead-120">3. Use the value of the **AutoDiscoverSMTPAddress** element returned in the Autodiscover response to [populate the value of the headers](#bk_setheadervalues).</span></span>  <br/> |
|<span data-ttu-id="4aead-121">**X-PublicFolderMailbox**</span><span class="sxs-lookup"><span data-stu-id="4aead-121">**X-PublicFolderMailbox**</span></span> <br/> |<span data-ttu-id="4aead-122">Votre travail est fini, la valeur X-PublicFolderMailbox est la même que la valeur X-AnchorMailbox !</span><span class="sxs-lookup"><span data-stu-id="4aead-122">Your work is done, the X-PublicFolderMailbox value is the same as the X-AnchorMailbox value!</span></span>  <br/> |<span data-ttu-id="4aead-123">Vous avez déjà fait !</span><span class="sxs-lookup"><span data-stu-id="4aead-123">You already have it!</span></span>  <br/> |
   
<span data-ttu-id="4aead-124">Une fois que vous avez déterminé les valeurs d’en-tête, incluez-les [lorsque vous effectuez des demandes de contenu de dossier public](#bk_setheadervalues).</span><span class="sxs-lookup"><span data-stu-id="4aead-124">After you have determined the header values, include them [when you make public folder content requests](#bk_setheadervalues).</span></span>
  
<span data-ttu-id="4aead-125">Les étapes décrites dans cet article sont spécifiques aux demandes de contenu de dossier public.</span><span class="sxs-lookup"><span data-stu-id="4aead-125">The steps in this article are specific to public folder content requests.</span></span> <span data-ttu-id="4aead-126">Pour déterminer si votre requête est une hiérarchie de dossiers publics ou une demande de contenu, consultez la rubrique [Routing Public Folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span><span class="sxs-lookup"><span data-stu-id="4aead-126">To determine whether your request is a public folder hierarchy or content request, see [Routing public folder requests](public-folder-access-with-ews-in-exchange.md#bk_routing).</span></span>

<span data-ttu-id="4aead-127"><a name="bk_determineguidewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4aead-127"><a name="bk_determineguidewsma"> </a></span></span>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a><span data-ttu-id="4aead-128">Déterminer le GUID de la boîte aux lettres de dossiers publics à l’aide de l’API managée EWS</span><span class="sxs-lookup"><span data-stu-id="4aead-128">Determine the GUID of the public folder mailbox by using the EWS Managed API</span></span>


<span data-ttu-id="4aead-129">Pour déterminer le GUID de la boîte aux lettres de contenu des dossiers publics, utilisez l’exemple de code suivant :</span><span class="sxs-lookup"><span data-stu-id="4aead-129">To determine the GUID of the public folder content mailbox, use the following code example, which does the following:</span></span> 
  
- <span data-ttu-id="4aead-130">Utilise les en-têtes **x-AnchorMailbox** et **x-PublicFolderInformation** que vous avez récupérés en [acheminant les requêtes de hiérarchie de dossiers publics](how-to-route-public-folder-hierarchy-requests.md).</span><span class="sxs-lookup"><span data-stu-id="4aead-130">Uses the **X-AnchorMailbox** and **X-PublicFolderInformation** headers you retrieved by [routing public folder hierarchy requests](how-to-route-public-folder-hierarchy-requests.md).</span></span>
    
- <span data-ttu-id="4aead-131">Appelle la méthode [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) de l’API managée EWS et inclut une demande pour la propriété **PR_REPLICA_LIST** (0x66980102)</span><span class="sxs-lookup"><span data-stu-id="4aead-131">Calls the EWS Managed API [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) method, and includes a request for the **PR_REPLICA_LIST** (0x66980102) property</span></span> 
    
<span data-ttu-id="4aead-132">La valeur **PR_REPLICA_LIST** identifie le GUID de boîte aux lettres de la boîte aux lettres de dossiers publics dont le contenu est associé au dossier.</span><span class="sxs-lookup"><span data-stu-id="4aead-132">The **PR_REPLICA_LIST** value identifies the mailbox GUID of the public folder mailbox that has the content for the folder.</span></span> <span data-ttu-id="4aead-133">La propriété **PR_REPLICA_LIST** est un tableau d’octets, mais est castée en tant que GUID pour ce scénario.</span><span class="sxs-lookup"><span data-stu-id="4aead-133">The **PR_REPLICA_LIST** property is a byte array, but is cast as a GUID for this scenario.</span></span> <span data-ttu-id="4aead-134">Le GUID et le nom de domaine sont concaténés pour former l’adresse sur laquelle appeler la découverte automatique.</span><span class="sxs-lookup"><span data-stu-id="4aead-134">The GUID and the domain name are concatenated to form the address on which to call Autodiscover.</span></span> 
  
<span data-ttu-id="4aead-135">Cet exemple suppose qu’il `service` s’agit de l’objet [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) pour l’utilisateur de boîte aux lettres et qu’il s’agit des `PFHAnchorHeader` `PFHMailboxHeader` valeurs des en-têtes **x-AnchorMailbox** et **x** , et que Domain est le nom de domaine utilisé par le client.</span><span class="sxs-lookup"><span data-stu-id="4aead-135">This example assumes that  `service` is the [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox user,  `PFHAnchorHeader` and  `PFHMailboxHeader` are the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers, and domain is the domain name used by the tenant.</span></span> 
  
```cs
public static string GetMailboxGuidAddress(ExchangeService service, String PFHAnchorHeader, String PFHMailboxHeader, String domain)
{
    // Create a new folder view, and pass in the maximum number of folders to return.
    FolderView view = new FolderView(10);
    // Create an extended property definition for the PR_REPLICA_LIST property.
    ExtendedPropertyDefinition PR_REPLICA_LIST = new ExtendedPropertyDefinition(0x6698, MapiPropertyType.Binary);
    // As a best practice, limit the properties returned to only those required.
    // In this case, return the folder ID, the folder display name, and 
    // the value of the PR_REPLICA_LIST extended property definition.
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, PR_REPLICA_LIST);
    service.HttpHeaders.Add("X-AnchorMailbox", PFHAnchorHeader);
    service.HttpHeaders.Add("X-PublicFolderMailbox", PFHMailboxHeader);
    // Add a call to the CertificateValidationCallback method here if needed.
    // ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;
    // Call FindFolders to retrieve the folder hierarchy, starting with the PublicFolderRoot folder.
    // This method call results in a FindFolder call to EWS.
    FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.PublicFoldersRoot, view);
    string GuidAsString = null;
    List<string> Guids = new List<string>();
    // For each folder under the root, display the name, and copy the value of the 
    // PR_REPLICA_LIST byte array to a string value. 
    foreach (Folder folder in findResults.Folders)
    {
        Console.WriteLine("Public folder display name: {0}", folder.DisplayName);
        byte[] ByteArr = (byte[])folder.ExtendedProperties[0].Value;
        GuidAsString = System.Text.Encoding.ASCII.GetString(ByteArr, 0, 36);
        Guids.Add(GuidAsString);
        Console.WriteLine("Address for Autodiscover: {0}.{1}\r\n", GuidAsString, domain);
    }
    // Concatenate the GUID value of the PR_REPLICA_LIST with the domain name to generate the 
    // SMTP address to use for the AutoDiscover request for the public folder content mailbox.
    string AutoDSMTPAddress = GuidAsString + "@" + domain;
    // Check that all folders have the same GUID value. If they do not, use the GUID value of the
    // folder that you're requesting content for.
    string commonGuid = CompareGuidsForEquality(Guids);
    if (commonGuid == "Not Equal")
    {
        Console.WriteLine("The GUIDs for all the folders in the hierarchy are not the same. Run the Autodiscover sample using the address returned above that is associated with the folder in your hierarchy request.", AutoDSMTPAddress);
        return null;
    }
    else
    {
        Console.WriteLine("The GUIDs for all public folders in the hierarchy are the same. Run the Autodiscover sample using the {0} address.", AutoDSMTPAddress);
        return AutoDSMTPAddress;
    }
}
// Method to compare the GUID for each folder under the public folder root.
// If each GUID is the same, return the GUID.
// If the GUIDs are not the same, return "Not equal".
public static string CompareGuidsForEquality(List<string> list)
{
    string NotEqual = "Not equal";
    string first = list.First();
    return list.All(x => x == first) ? first : NotEqual;
}
```

<span data-ttu-id="4aead-136">Si vous avez reçu l’erreur «la demande a échoué.</span><span class="sxs-lookup"><span data-stu-id="4aead-136">If you received the error "The request failed.</span></span> <span data-ttu-id="4aead-137">La connexion sous-jacente a été fermée : impossible d’établir une relation de confiance pour le canal sécurisé SSL/TLS ", vous devrez [Ajouter un appel à une méthode de rappel de validation](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="4aead-137">The underlying connection was closed: Could not establish trust relationship for the SSL/TLS secure channel", you'll need to [add a call to a validation callback method](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> <span data-ttu-id="4aead-138">Un espace réservé et un commentaire pour cette méthode sont inclus dans l’exemple de code.</span><span class="sxs-lookup"><span data-stu-id="4aead-138">A placeholder and comment for that method is included in the code example.</span></span>
  
<span data-ttu-id="4aead-139">Si le GUID de boîte aux lettres est le même pour tous les dossiers publics sous la racine de dossier public, l’exemple indique l’adresse à utiliser lors de l’appel de la [découverte automatique](#bk_makeautodrequest) dans la sortie de la console et en tant que valeur de retour.</span><span class="sxs-lookup"><span data-stu-id="4aead-139">If the mailbox GUID is the same for all the public folders under the public folder root, the example indicates the address to use when [calling Autodiscover](#bk_makeautodrequest) in the console output and as the return value.</span></span> <span data-ttu-id="4aead-140">Si le GUID de boîte aux lettres n’est pas le même pour tous les dossiers publics sous la racine de dossier public, vous devez [effectuer une demande de découverte automatique](#bk_makeautodrequest) sur l’adresse associée au dossier dans votre demande de contenu.</span><span class="sxs-lookup"><span data-stu-id="4aead-140">If the mailbox GUID is not the same for all public folders under the public folder root, you need to [Make an Autodiscover request](#bk_makeautodrequest) on the address associated with the folder in your content request.</span></span> 

<span data-ttu-id="4aead-141"><a name="bk_determineguidews"> </a></span><span class="sxs-lookup"><span data-stu-id="4aead-141"><a name="bk_determineguidews"> </a></span></span>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a><span data-ttu-id="4aead-142">Déterminer le GUID de la boîte aux lettres de dossiers publics à l’aide d’EWS</span><span class="sxs-lookup"><span data-stu-id="4aead-142">Determine the GUID of the public folder mailbox by using EWS</span></span>

<span data-ttu-id="4aead-143">L’exemple de code suivant montre comment extraire la valeur de la propriété **PR_REPLICA_LIST** (0x66980102) à l’aide de l’opération EWS [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4aead-143">The following code example shows how retrieve the value of the **PR_REPLICA_LIST** (0x66980102) property by using the EWS [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="4aead-144">Pour l' [élément ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) , l’attribut **PropertyTag** est défini sur la valeur décimale (26264) de la propriété **PR_REPLICA_LIST** et l’attribut **PropertyType** a la valeur **Binary**.</span><span class="sxs-lookup"><span data-stu-id="4aead-144">For the [ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) element, the **PropertyTag** attribute is set to the decimal value (26264) of the **PR_REPLICA_LIST** property, and the **PropertyType** attribute is set to **Binary**.</span></span>
  
<span data-ttu-id="4aead-145">Il s’agit également de la demande XML que l’API managée EWS envoie lorsque vous utilisez la méthode **FindFolders** pour [déterminer le GUID de la boîte aux lettres de dossiers publics à l’aide de l’API managée EWS](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="4aead-145">This is also the XML request that the EWS Managed API sends when you use the **FindFolders** method to [determine the GUID of the public folder mailbox by using the EWS Managed API](#bk_determineguidewsma).</span></span>
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0913.015
Accept-Encoding: gzip,deflate
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Cookie: ClientId=KZPBLKA9ZMPXAQDW
Content-Length: 1005
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="26264" PropertyType="Binary" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4aead-146">Le serveur répond à la demande **FindFolder** avec un message [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) qui inclut la valeur de la propriété étendue **PR_REPLICA_LIST** .</span><span class="sxs-lookup"><span data-stu-id="4aead-146">The server responds to the **FindFolder** request with a [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) message that includes the value of the **PR_REPLICA_LIST** extended property.</span></span> <span data-ttu-id="4aead-147">Notez que la valeur de la propriété apparaît sur la réponse EWS en tant que format de chaîne d’un tableau d’octets encodé en base 64.</span><span class="sxs-lookup"><span data-stu-id="4aead-147">Note that the value of the property appears on the EWS response as the string format of a base-64 encoded byte array.</span></span> <span data-ttu-id="4aead-148">Certaines valeurs d’en-tête dans la réponse sont raccourcies pour des raisons de lisibilité.</span><span class="sxs-lookup"><span data-stu-id="4aead-148">Some header values in the response are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" TotalItemsInView="2" IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="AAEuAAAAAADL8shaNEKnQYVvRbpoY9vDAQBGDloItRzyTrAt+XVzRr/YAABdofPkAAA=" ChangeKey="AwAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/2h"/>
                <t:DisplayName>My Public Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAxEAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/W/"/>
                <t:DisplayName>SampleFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="4aead-149">Afin d’utiliser la valeur de la **PR_REPLICA_LIST** renvoyée dans le fichier XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA = =, pour déterminer le GUID de boîte aux lettres, la valeur doit être convertie en GUID dans un format similaire à la façon dont la valeur est convertie dans l’exemple de code de l' [API managée EWS](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="4aead-149">In order to use the value of the **PR_REPLICA_LIST** returned in the XML, MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==, to determine the mailbox GUID, the value must be converted into a GUID in a format similar to how the value is converted in the [EWS Managed API code example](#bk_determineguidewsma).</span></span> <span data-ttu-id="4aead-150">Le GUID est ensuite concaténé avec le nom de domaine pour créer une adresse SMTP, qui est incluse dans la [demande de découverte automatique](#bk_makeautodrequest).</span><span class="sxs-lookup"><span data-stu-id="4aead-150">The GUID is then concatenated with the domain name to create an SMTP address, which is included in the [Autodiscover request](#bk_makeautodrequest).</span></span>
  
## <a name="make-an-autodiscover-request"></a><span data-ttu-id="4aead-151">Faire une demande de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="4aead-151">Make an Autodiscover request</span></span>
<span data-ttu-id="4aead-152"><a name="bk_makeautodrequest"> </a></span><span class="sxs-lookup"><span data-stu-id="4aead-152"><a name="bk_makeautodrequest"> </a></span></span>

<span data-ttu-id="4aead-153">Utilisez l’adresse renvoyée par la `GetMailboxGuidAddress` méthode pour appeler autodiscover.</span><span class="sxs-lookup"><span data-stu-id="4aead-153">Use the address returned by the  `GetMailboxGuidAddress` method to call Autodiscover.</span></span> <span data-ttu-id="4aead-154">Nous vous recommandons d’utiliser l’exemple de code [Exchange 2013 : Get User Settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) pour appeler le service de découverte automatique, car il simplifie le processus de découverte automatique pour vous.</span><span class="sxs-lookup"><span data-stu-id="4aead-154">We recommend that you use the [Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e) code sample to call the Autodiscover service because it streamlines the Autodiscover process for you.</span></span> <span data-ttu-id="4aead-155">Cet exemple de code utilise les arguments de ligne de commande figurant dans le tableau suivant pour appeler le service de découverte automatique POX afin de récupérer la valeur [AutoDiscoverSMTPAddress](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) associée au GUID de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4aead-155">This code sample uses the command-line arguments listed in the following table to call the POX Autodiscover service to retrieve the [AutoDiscoverSMTPAddress](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) value associated with the mailbox GUID.</span></span> 

  
|<span data-ttu-id="4aead-156">**Argument**</span><span class="sxs-lookup"><span data-stu-id="4aead-156">**Argument**</span></span>|<span data-ttu-id="4aead-157">**Description**</span><span class="sxs-lookup"><span data-stu-id="4aead-157">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4aead-158">emailAddress</span><span class="sxs-lookup"><span data-stu-id="4aead-158">emailAddress</span></span>  <br/> |<span data-ttu-id="4aead-159">Adresse renvoyée par la `GetMailboxGuidAddress` méthode dans [déterminer le GUID de la boîte aux lettres de dossiers publics](#bk_determineguidewsma).</span><span class="sxs-lookup"><span data-stu-id="4aead-159">The address returned by the  `GetMailboxGuidAddress` method in [Determine the GUID of the public folder mailbox](#bk_determineguidewsma).</span></span>  <br/> |
|<span data-ttu-id="4aead-160">-skipSOAP</span><span class="sxs-lookup"><span data-stu-id="4aead-160">-skipSOAP</span></span>  <br/> |<span data-ttu-id="4aead-161">Indique que les demandes de découverte automatique de POX sont requises.</span><span class="sxs-lookup"><span data-stu-id="4aead-161">Indicates that POX Autodiscover requests are required.</span></span>  <br/> |
|<span data-ttu-id="4aead-162">-authEmailAddress auth</span><span class="sxs-lookup"><span data-stu-id="4aead-162">-auth authEmailAddress</span></span>  <br/> |<span data-ttu-id="4aead-163">L’adresse de messagerie de l’utilisateur de la boîte aux lettres, qui est utilisée pour l’authentification.</span><span class="sxs-lookup"><span data-stu-id="4aead-163">The mailbox user's email address, which is used for authentication.</span></span> <span data-ttu-id="4aead-164">Vous serez invité à entrer le mot de passe de l’utilisateur de boîte aux lettres lors de l’exécution de l’exemple.</span><span class="sxs-lookup"><span data-stu-id="4aead-164">You will be prompted to enter the mailbox user's password when you run the sample.</span></span>  <br/> |
   
<span data-ttu-id="4aead-165">Par exemple, les arguments de ligne de commande doivent ressembler à ceci :</span><span class="sxs-lookup"><span data-stu-id="4aead-165">For example, the command-line arguments should look like this:</span></span>
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

<span data-ttu-id="4aead-166">Où `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` est l’adresse renvoyée par la méthode **GetMailboxGuidAddress** et `sonyaf@contoso.com` est l’utilisateur de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4aead-166">Where `1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` is the address returned by the **GetMailboxGuidAddress** method, and `sonyaf@contoso.com` is the mailbox user.</span></span> 
  
<span data-ttu-id="4aead-167">Lorsque vous exécutez l’exemple de code **Exchange 2013 : Get User Settings with Autodiscover** , la dernière réponse de découverte automatique doit réussir et inclure tous les paramètres utilisateur associés au GUID de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="4aead-167">When you run the **Exchange 2013: Get user settings with Autodiscover** sample, the last Autodiscover response should be successful and include all the user settings associated with the mailbox GUID.</span></span> <span data-ttu-id="4aead-168">Enregistrez le paramètre utilisateur **AutoDiscoverSMTPAddress** localement, comme vous l’utiliserez à l’étape suivante.</span><span class="sxs-lookup"><span data-stu-id="4aead-168">Save the **AutoDiscoverSMTPAddress** user setting locally, as you'll use that in the next step.</span></span> 
  
<span data-ttu-id="4aead-169">Sinon, si vous ne souhaitez pas utiliser **Exchange 2013 : Get User Settings with Autodiscover** Sample, vous pouvez obtenir le paramètre utilisateur **AutoDiscoverSMTPAddress** en [générant une liste de points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md), puis en envoyant la demande de découverte automatique pox suivante à chaque URL jusqu’à ce que vous receviez une réponse réussie.</span><span class="sxs-lookup"><span data-stu-id="4aead-169">Alternatively, if you do not want to use **Exchange 2013: Get user settings with Autodiscover** sample, you can get the **AutoDiscoverSMTPAddress** user setting by [generating a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and then sending the following POX Autodiscover request to each URL until you receive a successful response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

<span data-ttu-id="4aead-170">Pour plus d’informations sur le processus de découverte automatique, voir [Autodiscover pour Exchange](autodiscover-for-exchange.md), [générer une liste des points de terminaison de découverte automatique](how-to-generate-a-list-of-autodiscover-endpoints.md)et [obtenir les paramètres utilisateur à partir d’Exchange à l’aide de la découverte automatique](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span><span class="sxs-lookup"><span data-stu-id="4aead-170">For more information about the Autodiscover process, see [Autodiscover for Exchange](autodiscover-for-exchange.md), [Generate a list of Autodiscover endpoints](how-to-generate-a-list-of-autodiscover-endpoints.md), and [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md).</span></span>
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a><span data-ttu-id="4aead-171">Définir les valeurs des en-têtes X-AnchorMailbox et X-PublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="4aead-171">Set the values of the X-AnchorMailbox and X-PublicFolderMailbox headers</span></span>
<span data-ttu-id="4aead-172"><a name="bk_setheadervalues"> </a></span><span class="sxs-lookup"><span data-stu-id="4aead-172"><a name="bk_setheadervalues"> </a></span></span>

<span data-ttu-id="4aead-173">À l’aide de la valeur pour le **AutoDiscoverSMTPAddress** acquis dans [Make a Autodiscover Request](#bk_makeautodrequest), définissez les valeurs des en-têtes **x-AnchorMailbox** et **x** dans la demande de contenu de dossier public.</span><span class="sxs-lookup"><span data-stu-id="4aead-173">Using the value for the **AutoDiscoverSMTPAddress** acquired in [Make an Autodiscover request](#bk_makeautodrequest), set the values of the **X-AnchorMailbox** and **X-PublicFolderMailbox** headers in your public folder content request.</span></span> 
  
<span data-ttu-id="4aead-174">Par exemple, étant donné un AutoDiscoverSMTPAddress de NewPublicFolder@contoso.com, incluez les en-têtes suivants lors des appels aux méthodes ou opérations suivantes.</span><span class="sxs-lookup"><span data-stu-id="4aead-174">For example, given an AutoDiscoverSMTPAddress of NewPublicFolder@contoso.com, include the following headers when making calls to the following methods or operations.</span></span>
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

<span data-ttu-id="4aead-175">**Appels de dossier public nécessitant les en-têtes X-AncorMailbox et X-PublicFolder**</span><span class="sxs-lookup"><span data-stu-id="4aead-175">**Public folder calls that require the X-AncorMailbox and X-PublicFolder headers**</span></span>

|<span data-ttu-id="4aead-176">**Méthodes d'API managée EWS**</span><span class="sxs-lookup"><span data-stu-id="4aead-176">**EWS Managed API methods**</span></span>|<span data-ttu-id="4aead-177">**Opérations EWS**</span><span class="sxs-lookup"><span data-stu-id="4aead-177">**EWS operations**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4aead-178">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="4aead-178">Item.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="4aead-179">Item.Update</span><span class="sxs-lookup"><span data-stu-id="4aead-179">Item.Update</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="4aead-180">Item. Copy</span><span class="sxs-lookup"><span data-stu-id="4aead-180">Item.Copy</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="4aead-181">Item. Move</span><span class="sxs-lookup"><span data-stu-id="4aead-181">Item.Move</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="4aead-182">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="4aead-182">Item.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="4aead-183">Folder. bind</span><span class="sxs-lookup"><span data-stu-id="4aead-183">Folder.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="4aead-184">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="4aead-184">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4aead-185">CreateItem</span><span class="sxs-lookup"><span data-stu-id="4aead-185">CreateItem</span></span>](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [<span data-ttu-id="4aead-186">GetItem</span><span class="sxs-lookup"><span data-stu-id="4aead-186">GetItem</span></span>](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [<span data-ttu-id="4aead-187">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="4aead-187">UpdateItem</span></span>](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [<span data-ttu-id="4aead-188">CopyItem</span><span class="sxs-lookup"><span data-stu-id="4aead-188">CopyItem</span></span>](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [<span data-ttu-id="4aead-189">MoveItem</span><span class="sxs-lookup"><span data-stu-id="4aead-189">MoveItem</span></span>](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [<span data-ttu-id="4aead-190">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="4aead-190">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> [<span data-ttu-id="4aead-191">GetFolder</span><span class="sxs-lookup"><span data-stu-id="4aead-191">GetFolder</span></span>](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [<span data-ttu-id="4aead-192">FindItem</span><span class="sxs-lookup"><span data-stu-id="4aead-192">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="4aead-193">Pour ajouter ces en-têtes à l’aide de l’API managée EWS, utilisez la méthode [HttpHeaders. Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4aead-193">To add these headers by using the EWS Managed API, use the [HttpHeaders.Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) method.</span></span> 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

<span data-ttu-id="4aead-194">Le code suivant montre une demande [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) avec l’en-tête **x-AnchorMailbox** et **x-PublicFolderMailbox** défini sur les valeurs récupérées dans les exemples de cet article.</span><span class="sxs-lookup"><span data-stu-id="4aead-194">The following code shows a [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) request with the **X-AnchorMailbox** and **X-PublicFolderMailbox** header set to the values retrieved in the examples in this article.</span></span> 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: NewPublicFolder@contoso.com
X-PublicFolderMailbox: NewPublicFolder@contoso.com
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Content-Length: 688
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="4aead-195">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4aead-195">See also</span></span>

- [<span data-ttu-id="4aead-196">Accéder aux dossiers publics avec EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4aead-196">Public folder access with EWS in Exchange</span></span>](public-folder-access-with-ews-in-exchange.md)    
- [<span data-ttu-id="4aead-197">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="4aead-197">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)    
- [<span data-ttu-id="4aead-198">Générer une liste de points de terminaison de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="4aead-198">Generate a list of Autodiscover endpoints</span></span>](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [<span data-ttu-id="4aead-199">Obtenir les paramètres de l'utilisateur Exchange à l'aide de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="4aead-199">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
  