---
title: Opération ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: 6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb
description: Adresses de messagerie ambiguë ResolveNames opération résout les noms d’affichage.
ms.openlocfilehash: 8443cf834dfdf104daeaaa92fdee3742c3fa3719
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19829162"
---
# <a name="resolvenames-operation"></a><span data-ttu-id="10b3c-103">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="10b3c-103">ResolveNames operation</span></span>

<span data-ttu-id="10b3c-104">Adresses de messagerie ambiguë **ResolveNames** opération résout les noms d’affichage.</span><span class="sxs-lookup"><span data-stu-id="10b3c-104">The **ResolveNames** operation resolves ambiguous email addresses and display names.</span></span> 
  
## <a name="using-the-resolvenames-operation"></a><span data-ttu-id="10b3c-105">Utilisation de l’opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="10b3c-105">Using the ResolveNames operation</span></span>

<span data-ttu-id="10b3c-106">Cette opération peut être utilisée pour vérifier les alias et résoudre les noms d’affichage à l’utilisateur de boîte aux lettres appropriée.</span><span class="sxs-lookup"><span data-stu-id="10b3c-106">This operation can be used to verify aliases and resolve display names to the appropriate mailbox user.</span></span> <span data-ttu-id="10b3c-107">Si des noms ambigus existent, la réponse d’opération **ResolveNames** fournit des informations sur chaque utilisateur de boîte aux lettres afin que l’application cliente peut résoudre les noms.</span><span class="sxs-lookup"><span data-stu-id="10b3c-107">If ambiguous names exist, the **ResolveNames** operation response provides information about each mailbox user so that the client application can resolve the names.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="10b3c-108">Remarques</span><span class="sxs-lookup"><span data-stu-id="10b3c-108">Remarks</span></span>

<span data-ttu-id="10b3c-109">La réponse ResolveNames renvoie un maximum de 100 candidats.</span><span class="sxs-lookup"><span data-stu-id="10b3c-109">The ResolveNames response returns a maximum of 100 candidates.</span></span> <span data-ttu-id="10b3c-110">Les 100 candidats qui sont retournées sont les 100 premières lors de l’opération de recherche.</span><span class="sxs-lookup"><span data-stu-id="10b3c-110">The 100 candidates that are returned are the first 100 that are encountered in the lookup operation.</span></span>
  
<span data-ttu-id="10b3c-111">Adresses de messagerie avec des types de routage préfixés, tel que smtp ou sip, sont enregistrés dans un tableau à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="10b3c-111">Email addresses with prefixed routing types, such as smtp or sip, are saved in a multivalue array.</span></span> <span data-ttu-id="10b3c-112">L’opération **ResolveNames** effectue une correspondance partielle dans chaque valeur de ce tableau lorsque vous ajoutez le type de routage au début du nom non résolu, tel que « sip:User1@Contoso.com ».</span><span class="sxs-lookup"><span data-stu-id="10b3c-112">The **ResolveNames** operation performs a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1@Contoso.com".</span></span> <span data-ttu-id="10b3c-113">Si vous ne spécifiez pas un type de routage, **ResolveNames** par défaut pour le type de routage du service smtp, faire correspondre à une propriété d’adresse smtp principale et recherche pas dans le tableau à valeurs multiples.</span><span class="sxs-lookup"><span data-stu-id="10b3c-113">If you don't specify a routing type, **ResolveNames** will default to the routing type of smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> 
  
<span data-ttu-id="10b3c-114">Qu’un seul nom ambigu peut être spécifié dans une demande unique.</span><span class="sxs-lookup"><span data-stu-id="10b3c-114">Only one ambiguous name can be specified in a single request.</span></span> <span data-ttu-id="10b3c-115">Active Directory est recherché en premier, puis le dossier de contacts de l’utilisateur est recherché.</span><span class="sxs-lookup"><span data-stu-id="10b3c-115">Active Directory is searched first, and then the user's contact folder is searched.</span></span> <span data-ttu-id="10b3c-116">Résolu les entrées de dossier de contacts d’un utilisateur dont la propriété **ItemId** non null, qui peut ensuite être utilisée dans une requête GetItem.</span><span class="sxs-lookup"><span data-stu-id="10b3c-116">Resolved entries from a user's contact folder have a non-null **ItemId** property, which can then be used in a GetItem request.</span></span> <span data-ttu-id="10b3c-117">S’il s’agit de l’ID d’une liste de distribution privée, il peut être utilisé dans une [opération ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="10b3c-117">If it is the ID of a private distribution list, then it can be used in an [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="10b3c-118">Si l’attribut **ReturnFullContactData** est défini sur **true**, les entrées Active Directory avec l’opération **ResolveNames** renverra des propriétés supplémentaires qui décrivent un [Contact](contact.md).</span><span class="sxs-lookup"><span data-stu-id="10b3c-118">If the **ReturnFullContactData** attribute is set to **true**, then Active Directory entries found with the **ResolveNames** operation will return additional properties that describe a [Contact](contact.md).</span></span> <span data-ttu-id="10b3c-119">L’attribut **ReturnFullContactData** n’affecte pas les données qui sont retournées pour les contacts et privées des listes de distribution à partir du dossier de contacts de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="10b3c-119">The **ReturnFullContactData** attribute does not affect the data that is returned for contacts and private distribution lists from the user's contact folder.</span></span> 
  
## <a name="resolvenames-request-example"></a><span data-ttu-id="10b3c-120">Exemple de requête ResolveNames</span><span class="sxs-lookup"><span data-stu-id="10b3c-120">ResolveNames request example</span></span>

### <a name="description"></a><span data-ttu-id="10b3c-121">Description</span><span class="sxs-lookup"><span data-stu-id="10b3c-121">Description</span></span>

<span data-ttu-id="10b3c-122">L’exemple suivant d’une demande **ResolveNames** indique comment faire pour résoudre l’entrée de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="10b3c-122">The following example of a **ResolveNames** request shows how to resolve the entry of User.</span></span>
  
### <a name="code"></a><span data-ttu-id="10b3c-123">Code</span><span class="sxs-lookup"><span data-stu-id="10b3c-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>User2</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="10b3c-124">Commentaires</span><span class="sxs-lookup"><span data-stu-id="10b3c-124">Comments</span></span>

<span data-ttu-id="10b3c-125">La réponse à cette demande retournera toutes les entrées qui commencent par « Jo » ou « Mi ».</span><span class="sxs-lookup"><span data-stu-id="10b3c-125">The response to this request will return all entries that start with "Jo" or "Mi."</span></span> <span data-ttu-id="10b3c-126">Les éléments retournés sont publics boîtes aux lettres, les listes de distribution publiques et privées et les contacts.</span><span class="sxs-lookup"><span data-stu-id="10b3c-126">The returned items are public mailboxes, public and private distribution lists, and contacts.</span></span>
  
> [!NOTE]
> <span data-ttu-id="10b3c-127">Seuls les contacts dans le dossier Contacts personnel sont recherchés.</span><span class="sxs-lookup"><span data-stu-id="10b3c-127">Only contacts in the default personal Contacts folder are searched.</span></span> 
  
<span data-ttu-id="10b3c-128">Les résultats d’une requête **ResolveNames** possibles sont les suivantes :</span><span class="sxs-lookup"><span data-stu-id="10b3c-128">The following are the possible results for a **ResolveNames** request:</span></span> 
  
- <span data-ttu-id="10b3c-129">Réponses qui ne contiennent pas une entité résolue renvoie une valeur d’attribut **ResponseClass** égale à **l’erreur**.</span><span class="sxs-lookup"><span data-stu-id="10b3c-129">Responses that do not contain a resolved entity will return a **ResponseClass** attribute value equal to **Error**.</span></span> <span data-ttu-id="10b3c-130">L’élément **MessageText** contiendra « **aucun résultat n’est trouvé**. »</span><span class="sxs-lookup"><span data-stu-id="10b3c-130">The **MessageText** element will contain " **No results are found**."</span></span>
    
- <span data-ttu-id="10b3c-131">Réponses qui contiennent une seule entité résolue renvoie une valeur d’attribut **ResponseClass** égale à la **Réussite**.</span><span class="sxs-lookup"><span data-stu-id="10b3c-131">Responses that contain a single resolved entity will return a **ResponseClass** attribute value equal to **Success**.</span></span>
    
- <span data-ttu-id="10b3c-132">Réponses qui contiennent plusieurs entités possibles renvoie une valeur d’attribut **ResponseClass** égale à **Avertissement**.</span><span class="sxs-lookup"><span data-stu-id="10b3c-132">Responses that contain multiple possible entities will return a **ResponseClass** attribute value equal to **Warning**.</span></span> <span data-ttu-id="10b3c-133">Dans ce cas, l’entité pas pu être résolue vers une identité unique.</span><span class="sxs-lookup"><span data-stu-id="10b3c-133">In this case, the entity could not be resolved to a unique identity.</span></span> <span data-ttu-id="10b3c-134">L’élément **MessageText** contiendra « plusieurs résultats sont trouvent. »</span><span class="sxs-lookup"><span data-stu-id="10b3c-134">The **MessageText** element will contain "Multiple results are found."</span></span> 
    
### <a name="request-elements"></a><span data-ttu-id="10b3c-135">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="10b3c-135">Request elements</span></span>

<span data-ttu-id="10b3c-136">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="10b3c-136">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="10b3c-137">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="10b3c-137">ResolveNames</span></span>](resolvenames.md)
    
- [<span data-ttu-id="10b3c-138">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="10b3c-138">UnresolvedEntry</span></span>](unresolvedentry.md)
    
## <a name="successful-resolvenames-operation-response-example"></a><span data-ttu-id="10b3c-139">Exemple de réponse opération ResolveNames réussie</span><span class="sxs-lookup"><span data-stu-id="10b3c-139">Successful ResolveNames operation response example</span></span>

### <a name="description"></a><span data-ttu-id="10b3c-140">Description</span><span class="sxs-lookup"><span data-stu-id="10b3c-140">Description</span></span>

<span data-ttu-id="10b3c-141">L’exemple suivant montre une réponse positive à une demande **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="10b3c-141">The following example shows a successful response to a **ResolveNames** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="10b3c-142">Code</span><span class="sxs-lookup"><span data-stu-id="10b3c-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>User2</t:Name>
                <t:EmailAddress>User2@example.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>User2</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:User2@example.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-resolvenames-response-elements"></a><span data-ttu-id="10b3c-143">Éléments de réponse ResolveNames réussies</span><span class="sxs-lookup"><span data-stu-id="10b3c-143">Successful ResolveNames response elements</span></span>

<span data-ttu-id="10b3c-144">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="10b3c-144">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="10b3c-145">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="10b3c-145">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="10b3c-146">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="10b3c-146">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="10b3c-147">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="10b3c-147">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="10b3c-148">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="10b3c-148">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="10b3c-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="10b3c-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="10b3c-150">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="10b3c-150">ResolutionSet</span></span>](resolutionset.md)
    
- [<span data-ttu-id="10b3c-151">Solution</span><span class="sxs-lookup"><span data-stu-id="10b3c-151">Resolution</span></span>](resolution.md)
    
- [<span data-ttu-id="10b3c-152">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="10b3c-152">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="10b3c-153">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="10b3c-153">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="10b3c-154">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="10b3c-154">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="10b3c-155">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="10b3c-155">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="10b3c-156">MailboxType</span><span class="sxs-lookup"><span data-stu-id="10b3c-156">MailboxType</span></span>](mailboxtype.md)
    
- [<span data-ttu-id="10b3c-157">Contact</span><span class="sxs-lookup"><span data-stu-id="10b3c-157">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="10b3c-158">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="10b3c-158">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="10b3c-159">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="10b3c-159">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="10b3c-160">Entrée (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="10b3c-160">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
- [<span data-ttu-id="10b3c-161">ContactSource</span><span class="sxs-lookup"><span data-stu-id="10b3c-161">ContactSource</span></span>](contactsource.md)
    
## <a name="resolvenames-operation-error-response"></a><span data-ttu-id="10b3c-162">Réponse d’erreur ResolveNames opération</span><span class="sxs-lookup"><span data-stu-id="10b3c-162">ResolveNames operation error response</span></span>

### <a name="description"></a><span data-ttu-id="10b3c-163">Description</span><span class="sxs-lookup"><span data-stu-id="10b3c-163">Description</span></span>

<span data-ttu-id="10b3c-164">L’exemple suivant montre une réponse d’erreur à une demande **ResolveNames** .</span><span class="sxs-lookup"><span data-stu-id="10b3c-164">The following example shows an error response to a **ResolveNames** request.</span></span> <span data-ttu-id="10b3c-165">L’erreur est provoquée par tente de résoudre un nom qui ne peut pas être résolu.</span><span class="sxs-lookup"><span data-stu-id="10b3c-165">The error is caused by trying to resolve a name that cannot be resolved.</span></span> 
  
### <a name="code"></a><span data-ttu-id="10b3c-166">Code</span><span class="sxs-lookup"><span data-stu-id="10b3c-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="10b3c-167">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="10b3c-167">Error response elements</span></span>

<span data-ttu-id="10b3c-168">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="10b3c-168">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="10b3c-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="10b3c-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="10b3c-170">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="10b3c-170">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
    
- [<span data-ttu-id="10b3c-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="10b3c-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="10b3c-172">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="10b3c-172">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
    
- [<span data-ttu-id="10b3c-173">MessageText</span><span class="sxs-lookup"><span data-stu-id="10b3c-173">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="10b3c-174">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="10b3c-174">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="10b3c-175">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="10b3c-175">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="10b3c-176">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="10b3c-176">See also</span></span>



[<span data-ttu-id="10b3c-177">Opération ExpandDL</span><span class="sxs-lookup"><span data-stu-id="10b3c-177">ExpandDL operation</span></span>](expanddl-operation.md)


[<span data-ttu-id="10b3c-178">À l’aide de la résolution de noms</span><span class="sxs-lookup"><span data-stu-id="10b3c-178">Using Name Resolution</span></span>](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

