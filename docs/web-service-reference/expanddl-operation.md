---
title: Opération ExpandDL
manager: sethgros
ms.date: 07/27/2018
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: L’opération ExpandDL expose l’appartenance complète des listes de distribution.
ms.openlocfilehash: 8edaf057538e2c1136465f0ff7937c14477b2c47
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454049"
---
# <a name="expanddl-operation"></a><span data-ttu-id="14c36-103">Opération ExpandDL</span><span class="sxs-lookup"><span data-stu-id="14c36-103">ExpandDL operation</span></span>

<span data-ttu-id="14c36-104">L’opération ExpandDL expose l’appartenance complète des listes de distribution.</span><span class="sxs-lookup"><span data-stu-id="14c36-104">The ExpandDL operation exposes the full membership of distribution lists.</span></span>
  
## <a name="using-the-expanddl-web-method"></a><span data-ttu-id="14c36-105">Utilisation de la méthode Web ExpandDL</span><span class="sxs-lookup"><span data-stu-id="14c36-105">Using the ExpandDL Web Method</span></span>

<span data-ttu-id="14c36-106">L’opération ExpandDL utilise le service Web qui se trouve dans Exchange. asmx.</span><span class="sxs-lookup"><span data-stu-id="14c36-106">The ExpandDL operation uses the Web service that is located in Exchange.asmx.</span></span> <span data-ttu-id="14c36-107">Cette méthode de service Web accepte un élément de [boîte aux lettres](mailbox.md) qui peut contenir un élément enfant [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) pour l’expansion d’une liste de distribution publique ou un élément enfant [ItemId](itemid.md) pour l’expansion d’une liste de distribution privée.</span><span class="sxs-lookup"><span data-stu-id="14c36-107">This Web service method accepts a [Mailbox](mailbox.md) element that can contain either an [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) child element for an expansion of a public distribution list or an [ItemId](itemid.md) child element for the expansion of a private distribution list.</span></span> 
  
<span data-ttu-id="14c36-108">Les listes de distribution publiques peuvent être étendues à l’aide de l’une des méthodes suivantes :</span><span class="sxs-lookup"><span data-stu-id="14c36-108">Public distribution lists can be expanded by using one of the following:</span></span>
  
1. <span data-ttu-id="14c36-109">Alias de liste de distribution</span><span class="sxs-lookup"><span data-stu-id="14c36-109">Distribution list alias</span></span>
    
2. <span data-ttu-id="14c36-110">Adresse du service SMTP (Simple Mail Transfer Protocol)</span><span class="sxs-lookup"><span data-stu-id="14c36-110">The Simple Mail Transfer Protocol (SMTP) address</span></span>
    
3. <span data-ttu-id="14c36-111">X400</span><span class="sxs-lookup"><span data-stu-id="14c36-111">X400</span></span>
    
4. <span data-ttu-id="14c36-112">X500</span><span class="sxs-lookup"><span data-stu-id="14c36-112">X500</span></span>
    
5. <span data-ttu-id="14c36-113">Adresse héritée Exchange</span><span class="sxs-lookup"><span data-stu-id="14c36-113">Exchange Legacy address</span></span>
    
6. <span data-ttu-id="14c36-114">Nom de la liste de distribution</span><span class="sxs-lookup"><span data-stu-id="14c36-114">The distribution list name</span></span>
    
7. <span data-ttu-id="14c36-115">Nom d’affichage</span><span class="sxs-lookup"><span data-stu-id="14c36-115">The display name</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="14c36-116">Les noms d’affichage ne sont pas uniques.</span><span class="sxs-lookup"><span data-stu-id="14c36-116">Display names are not unique.</span></span> <span data-ttu-id="14c36-117">Plusieurs comptes peuvent partager le même nom complet.</span><span class="sxs-lookup"><span data-stu-id="14c36-117">Multiple accounts can share the same display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="14c36-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="14c36-118">Remarks</span></span>

<span data-ttu-id="14c36-119">L’expansion récursive n’est pas prise en charge.</span><span class="sxs-lookup"><span data-stu-id="14c36-119">Recursive expansion is not supported.</span></span> <span data-ttu-id="14c36-120">Une seule liste de distribution peut être étendue en un seul appel.</span><span class="sxs-lookup"><span data-stu-id="14c36-120">Only one distribution list can be expanded in a single call.</span></span> <span data-ttu-id="14c36-121">Si plusieurs listes de distribution correspondent aux critères, le service Web signale une erreur.</span><span class="sxs-lookup"><span data-stu-id="14c36-121">If more than one distribution list match the criteria, the Web service reports an error.</span></span> <span data-ttu-id="14c36-122">Une application cliente peut utiliser la résolution de nom ambigu pour rechercher des listes de distribution ambiguës, puis choisir l’adresse de messagerie correcte de la liste de distribution requise en tant que paramètre pour l' [opération ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="14c36-122">A client application can use ambiguous name resolution (ANR) to find ambiguous distribution lists and then chose the correct e-mail address of the required distribution list as a parameter for the [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="14c36-123">Pour plus d’informations, consultez la rubrique [operation ResolveNames](resolvenames-operation.md).</span><span class="sxs-lookup"><span data-stu-id="14c36-123">For more information, see [ResolveNames operation](resolvenames-operation.md).</span></span>
  
<span data-ttu-id="14c36-124">Les listes de distribution publiques se trouvent dans Active Directory.</span><span class="sxs-lookup"><span data-stu-id="14c36-124">Public distribution lists are located in Active Directory.</span></span> <span data-ttu-id="14c36-125">Il peut s’agir de n’importe quel groupe de distribution dynamique ou à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="14c36-125">They can be any mail-enabled or dynamic distribution group.</span></span> <span data-ttu-id="14c36-126">Le groupe ne doit pas être masqué dans la liste d’adresses et chaque membre doit avoir une adresse de messagerie non vide.</span><span class="sxs-lookup"><span data-stu-id="14c36-126">The group should not be hidden from the address list and each member should have a non-empty e-mail address.</span></span> <span data-ttu-id="14c36-127">Les membres de la liste de distribution peuvent être des utilisateurs et des contacts à extension messagerie, des dossiers publics, ainsi que des listes de distribution et des groupes dynamiques à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="14c36-127">Members of the distribution list can be mail-enabled users and contacts, public folders, and mail-enabled distribution lists and dynamic groups.</span></span>
  
<span data-ttu-id="14c36-128">Les listes de distribution privées se trouvent dans le dossier contacts de la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="14c36-128">Private distribution lists are located in the Contacts folder of a user's mailbox.</span></span> <span data-ttu-id="14c36-129">Les listes de distribution privées n’ont pas d’adresses de messagerie pour que leurs identificateurs d’élément de magasin soient utilisés dans une demande ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="14c36-129">Private distribution lists do not have e-mail addresses so their store item identifiers are used in an ExpandDL request.</span></span> <span data-ttu-id="14c36-130">Les membres d’une liste de distribution privée peuvent être des utilisateurs à extension messagerie, des contacts ou des listes de distribution d’Active Directory, ou des listes de distribution de contacts ou privées à partir du dossier de contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="14c36-130">Members of a private distribution list can be any mail-enabled user, contacts or distribution lists from Active Directory, or contacts or private distribution lists from a user's Contacts folder.</span></span>
  
<span data-ttu-id="14c36-131">Pour les contacts ou les listes de distribution privées, les identificateurs d’élément sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="14c36-131">For contacts or private distribution lists, the item identifiers are returned in the response.</span></span> <span data-ttu-id="14c36-132">Cela peut être utilisé pour obtenir des informations sur l’objet ou pour développer l’appartenance à une liste de distribution privée.</span><span class="sxs-lookup"><span data-stu-id="14c36-132">This can be used to get information about the object or to expand membership in a private distribution list.</span></span>
  
## <a name="expanddl-private-distribution-list-request-example"></a><span data-ttu-id="14c36-133">Exemple de requête de liste de distribution privée ExpandDL</span><span class="sxs-lookup"><span data-stu-id="14c36-133">ExpandDL Private Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="14c36-134">Description</span><span class="sxs-lookup"><span data-stu-id="14c36-134">Description</span></span>

<span data-ttu-id="14c36-135">L’exemple de requête ExpandDL suivant montre comment créer une demande pour développer une liste de distribution privée.</span><span class="sxs-lookup"><span data-stu-id="14c36-135">The following example of an ExpandDL request shows how to form a request to expand a private distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="14c36-136">Code</span><span class="sxs-lookup"><span data-stu-id="14c36-136">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ExpandDL>
      <m:Mailbox>
       <t:EmailAddress>test</t:EmailAddress>
      </m:Mailbox>
    </m:ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="14c36-137">Commentaires</span><span class="sxs-lookup"><span data-stu-id="14c36-137">Comments</span></span>

<span data-ttu-id="14c36-138">Pour développer une liste de distribution privée, l’élément [Mailbox](mailbox.md) contient l’élément [ItemId](itemid.md) qui identifie une liste de distribution privée dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="14c36-138">To expand a private distribution list, the [Mailbox](mailbox.md) element will contain the [ItemId](itemid.md) element that identifies a private distribution list in the user's mailbox.</span></span> 
  
## <a name="expanddl-public-distribution-list-request-example"></a><span data-ttu-id="14c36-139">Exemple de requête de liste de distribution publique ExpandDL</span><span class="sxs-lookup"><span data-stu-id="14c36-139">ExpandDL Public Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="14c36-140">Description</span><span class="sxs-lookup"><span data-stu-id="14c36-140">Description</span></span>

<span data-ttu-id="14c36-141">L’exemple de requête ExpandDL suivant montre comment créer une demande pour développer une liste de distribution publique.</span><span class="sxs-lookup"><span data-stu-id="14c36-141">The following example of an ExpandDL request shows how to form a request to expand a public distribution list.</span></span> <span data-ttu-id="14c36-142">L’exemple illustre l’utilisation d’un nom d’affichage pour développer une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="14c36-142">The example shows the use of a display name to expand a distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="14c36-143">Code</span><span class="sxs-lookup"><span data-stu-id="14c36-143">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="14c36-144">Commentaires</span><span class="sxs-lookup"><span data-stu-id="14c36-144">Comments</span></span>

<span data-ttu-id="14c36-145">La réponse à cette demande contiendra des éléments de **boîte aux** lettres qui identifient chaque boîte aux lettres dans la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="14c36-145">The response to this request will contain **Mailbox** elements that identify each mailbox in the distribution list.</span></span> <span data-ttu-id="14c36-146">Si une liste de distribution est contenue dans une liste de distribution, un développement de liste de distribution distinct doit être effectué sur la liste de distribution incorporée.</span><span class="sxs-lookup"><span data-stu-id="14c36-146">If a distribution list is contained within a distribution list, a separate distribution list expansion must be performed on the embedded distribution list.</span></span> <span data-ttu-id="14c36-147">Si la liste de distribution n’a pas de membres ou si la liste de distribution demandée n’existe pas, l’attribut **ResponseClass** contient une valeur égale à success.</span><span class="sxs-lookup"><span data-stu-id="14c36-147">If the distribution list has no members or the requested distribution list does not exist, the **ResponseClass** attribute will contain a value equal to Success.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="14c36-148">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="14c36-148">Request elements</span></span>

<span data-ttu-id="14c36-149">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="14c36-149">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="14c36-150">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="14c36-150">ExpandDL</span></span>](expanddl.md)
    
- [<span data-ttu-id="14c36-151">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="14c36-151">Mailbox</span></span>](mailbox.md)
    
- <span data-ttu-id="14c36-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est utilisé pour identifier les listes de distribution publiques.</span><span class="sxs-lookup"><span data-stu-id="14c36-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) is used to identify public distribution lists.</span></span> <span data-ttu-id="14c36-153">L’élément [ItemId](itemid.md) est utilisé pour identifier les listes de distribution privées.</span><span class="sxs-lookup"><span data-stu-id="14c36-153">The [ItemId](itemid.md) element is used to identify private distribution lists.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="14c36-154">Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="14c36-154">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-expanddl-response-example"></a><span data-ttu-id="14c36-155">Exemple de réponse ExpandDL réussi</span><span class="sxs-lookup"><span data-stu-id="14c36-155">Successful ExpandDL response example</span></span>

### <a name="description"></a><span data-ttu-id="14c36-156">Description</span><span class="sxs-lookup"><span data-stu-id="14c36-156">Description</span></span>

<span data-ttu-id="14c36-157">L’exemple suivant de réponse ExpandDL indique une réponse à la demande décrite ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="14c36-157">The following example of an ExpandDL response shows a response to the request described above.</span></span> <span data-ttu-id="14c36-158">L’expansion de la liste de distribution décrit les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="14c36-158">The distribution list expansion describes the following:</span></span> 
  
- <span data-ttu-id="14c36-159">Nombre de membres de la liste de distribution qui sont renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="14c36-159">The number of members of the distribution list that are returned in the response.</span></span>
    
- <span data-ttu-id="14c36-160">Indique si la réponse contient tous les membres de la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="14c36-160">Whether the response contains all the members of the distribution list.</span></span>
    
- <span data-ttu-id="14c36-161">Nom de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="14c36-161">The name of the mailbox.</span></span>
    
- <span data-ttu-id="14c36-162">Adresse de messagerie de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="14c36-162">The e-mail address of the mailbox.</span></span>
    
- <span data-ttu-id="14c36-163">Type de routage de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="14c36-163">The routing type for the mailbox.</span></span>
    
- <span data-ttu-id="14c36-164">Type de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="14c36-164">The type of mailbox.</span></span>
    
> [!NOTE]
> <span data-ttu-id="14c36-165">Le nom de la liste de distribution n’est pas inclus dans la réponse ; par conséquent, vous devez effectuer le suivi du nom de la demande.</span><span class="sxs-lookup"><span data-stu-id="14c36-165">The distribution list name is not included in the response; therefore, you must keep track of the name from the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="14c36-166">Code</span><span class="sxs-lookup"><span data-stu-id="14c36-166">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DLExpansion TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Mailbox>
              <t:Name>Dan Park</t:Name>
              <t:EmailAddress>dpark@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Jeff Price</t:Name>
              <t:EmailAddress>jprice@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
            <t:Mailbox>
              <t:Name>Tanja Plate</t:Name>
              <t:EmailAddress>tplate@exampledomain.com</t:EmailAddress>
              <t:RoutingType>SMTP</t:RoutingType>
              <t:MailboxType>Mailbox</t:MailboxType>
            </t:Mailbox>
          </m:DLExpansion>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="14c36-167">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="14c36-167">Successful response elements</span></span>

<span data-ttu-id="14c36-168">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="14c36-168">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="14c36-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="14c36-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="14c36-170">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="14c36-170">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="14c36-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="14c36-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="14c36-172">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="14c36-172">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="14c36-173">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="14c36-173">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="14c36-174">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="14c36-174">DLExpansion</span></span>](dlexpansion.md)
    
- [<span data-ttu-id="14c36-175">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="14c36-175">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="14c36-176">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="14c36-176">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="14c36-177">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="14c36-177">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="14c36-178">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="14c36-178">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="14c36-179">MailboxType</span><span class="sxs-lookup"><span data-stu-id="14c36-179">MailboxType</span></span>](mailboxtype.md)
    
<span data-ttu-id="14c36-180">Pour trouver d’autres options pour le message de réponse de l’opération ExpandDL, explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="14c36-180">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="14c36-181">Commencez par l’élément [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="14c36-181">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="expanddl-error-response"></a><span data-ttu-id="14c36-182">Réponse d’erreur ExpandDL</span><span class="sxs-lookup"><span data-stu-id="14c36-182">ExpandDL error response</span></span>

### <a name="description"></a><span data-ttu-id="14c36-183">Description</span><span class="sxs-lookup"><span data-stu-id="14c36-183">Description</span></span>

<span data-ttu-id="14c36-184">L’exemple suivant montre une réponse d’erreur à une demande ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="14c36-184">The following example shows an error response to an ExpandDL request.</span></span>
  
### <a name="code"></a><span data-ttu-id="14c36-185">Code</span><span class="sxs-lookup"><span data-stu-id="14c36-185">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ExpandDLResponseMessage ResponseClass="Error">
          <m:MessageText>No results are found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ExpandDLResponseMessage>
      </m:ResponseMessages>
    </ExpandDLResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="14c36-186">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="14c36-186">Error response elements</span></span>

<span data-ttu-id="14c36-187">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="14c36-187">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="14c36-188">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="14c36-188">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="14c36-189">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="14c36-189">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="14c36-190">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="14c36-190">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="14c36-191">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="14c36-191">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="14c36-192">MessageText</span><span class="sxs-lookup"><span data-stu-id="14c36-192">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="14c36-193">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="14c36-193">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="14c36-194">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="14c36-194">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="14c36-195">Pour trouver d’autres options pour le message de réponse de l’opération ExpandDL, explorez la hiérarchie du schéma.</span><span class="sxs-lookup"><span data-stu-id="14c36-195">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="14c36-196">Commencez par l’élément [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="14c36-196">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="14c36-197">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="14c36-197">See also</span></span>

- [<span data-ttu-id="14c36-198">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="14c36-198">ResolveNames operation</span></span>](resolvenames-operation.md)
- [<span data-ttu-id="14c36-199">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="14c36-199">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

