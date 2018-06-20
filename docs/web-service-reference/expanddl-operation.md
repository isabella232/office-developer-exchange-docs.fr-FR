---
title: Opération ExpandDL
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDL
api_type:
- schema
ms.assetid: 1f7837e7-9eff-4e10-9577-c40f7ed6af94
description: L’opération ExpandDL expose tous les membres des listes de distribution.
ms.openlocfilehash: e4654120881f81a79358e0e7c0ab016f94db3288
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756263"
---
# <a name="expanddl-operation"></a><span data-ttu-id="7e3bd-103">Opération ExpandDL</span><span class="sxs-lookup"><span data-stu-id="7e3bd-103">ExpandDL operation</span></span>

<span data-ttu-id="7e3bd-104">L’opération ExpandDL expose tous les membres des listes de distribution.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-104">The ExpandDL operation exposes the full membership of distribution lists.</span></span>
  
## <a name="using-the-expanddl-web-method"></a><span data-ttu-id="7e3bd-105">À l’aide de la méthode Web ExpandDL</span><span class="sxs-lookup"><span data-stu-id="7e3bd-105">Using the ExpandDL Web Method</span></span>

<span data-ttu-id="7e3bd-106">L’opération ExpandDL utilise le service Web qui se trouve dans Exchange.asmx.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-106">The ExpandDL operation uses the Web service that is located in Exchange.asmx.</span></span> <span data-ttu-id="7e3bd-107">Cette méthode de service Web accepte un élément de [boîte aux lettres](mailbox.md) qui peut contenir un élément enfant de [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) pour une extension d’une liste de distribution publique ou un élément enfant de [ItemId](itemid.md) pour le développement de privé liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-107">This Web service method accepts a [Mailbox](mailbox.md) element that can contain either an [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) child element for an expansion of a public distribution list or an [ItemId](itemid.md) child element for the expansion of a private distribution list.</span></span> 
  
<span data-ttu-id="7e3bd-108">Listes de distribution publiques peuvent être développés à l’aide d’une des options suivantes :</span><span class="sxs-lookup"><span data-stu-id="7e3bd-108">Public distribution lists can be expanded by using one of the following:</span></span>
  
1. <span data-ttu-id="7e3bd-109">Alias de liste de distribution</span><span class="sxs-lookup"><span data-stu-id="7e3bd-109">Distribution list alias</span></span>
    
2. <span data-ttu-id="7e3bd-110">L’adresse SMTP Simple Mail Transfer Protocol)</span><span class="sxs-lookup"><span data-stu-id="7e3bd-110">The Simple Mail Transfer Protocol (SMTP) address</span></span>
    
3. <span data-ttu-id="7e3bd-111">X400</span><span class="sxs-lookup"><span data-stu-id="7e3bd-111">X400</span></span>
    
4. <span data-ttu-id="7e3bd-112">X500</span><span class="sxs-lookup"><span data-stu-id="7e3bd-112">X500</span></span>
    
5. <span data-ttu-id="7e3bd-113">Adresse Exchange hérité</span><span class="sxs-lookup"><span data-stu-id="7e3bd-113">Exchange Legacy address</span></span>
    
6. <span data-ttu-id="7e3bd-114">Nom de la liste de distribution</span><span class="sxs-lookup"><span data-stu-id="7e3bd-114">The distribution list name</span></span>
    
7. <span data-ttu-id="7e3bd-115">Le nom complet</span><span class="sxs-lookup"><span data-stu-id="7e3bd-115">The display name</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="7e3bd-116">Noms complets ne sont pas uniques.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-116">Display names are not unique.</span></span> <span data-ttu-id="7e3bd-117">Comptes multiples peuvent partager le même nom complet.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-117">Multiple accounts can share the same display name.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7e3bd-118">Remarques</span><span class="sxs-lookup"><span data-stu-id="7e3bd-118">Remarks</span></span>

<span data-ttu-id="7e3bd-119">Le développement récursive n’est pas pris en charge.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-119">Recursive expansion is not supported.</span></span> <span data-ttu-id="7e3bd-120">Liste de distribution qu’un seul peut être développée dans un seul appel.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-120">Only one distribution list can be expanded in a single call.</span></span> <span data-ttu-id="7e3bd-121">Si plusieurs listes de distribution correspondant aux critères, le service Web signale une erreur.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-121">If more than one distribution list match the criteria, the Web service reports an error.</span></span> <span data-ttu-id="7e3bd-122">Une application cliente permet la résolution de nom ambigu (ANR) pour trouver distribution ambigüe répertorie, puis sur l’adresse de messagerie de la liste de distribution requis en tant que paramètre de l' [opération ExpandDL](expanddl-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7e3bd-122">A client application can use ambiguous name resolution (ANR) to find ambiguous distribution lists and then chose the correct e-mail address of the required distribution list as a parameter for the [ExpandDL operation](expanddl-operation.md).</span></span> <span data-ttu-id="7e3bd-123">Pour plus d’informations, voir [opération ResolveNames](resolvenames-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7e3bd-123">For more information, see [ResolveNames operation](resolvenames-operation.md).</span></span>
  
<span data-ttu-id="7e3bd-124">Listes de distribution publiques sont situés dans Active Directory.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-124">Public distribution lists are located in Active Directory.</span></span> <span data-ttu-id="7e3bd-125">Ils peuvent être n’importe quel groupe de distribution dynamique ou à extension messagerie.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-125">They can be any mail-enabled or dynamic distribution group.</span></span> <span data-ttu-id="7e3bd-126">Le groupe ne doit pas être masqué à partir de la liste d’adresses et chaque membre doit avoir une adresse de messagerie non vides.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-126">The group should not be hidden from the address list and each member should have a non-empty e-mail address.</span></span> <span data-ttu-id="7e3bd-127">Membres de la liste de distribution peuvent être des utilisateurs à extension messagerie et de contacts, les dossiers publics et les listes de distribution à extension messagerie et groupes dynamiques.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-127">Members of the distribution list can be mail-enabled users and contacts, public folders, and mail-enabled distribution lists and dynamic groups.</span></span>
  
<span data-ttu-id="7e3bd-128">Listes de distribution privée se trouvent dans le dossier Contacts de boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-128">Private distribution lists are located in the Contacts folder of a user's mailbox.</span></span> <span data-ttu-id="7e3bd-129">Listes de distribution privée n’ont pas d’adresses de messagerie pour leurs identificateurs d’élément de magasin sont utilisés dans une requête ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-129">Private distribution lists do not have e-mail addresses so their store item identifiers are used in an ExpandDL request.</span></span> <span data-ttu-id="7e3bd-130">Membres d’une liste de distribution privée peuvent être n’importe quel utilisateur à extension messagerie, les contacts ou les listes de distribution à partir d’Active Directory ou les listes de contacts ou distribution privée à partir du dossier de Contacts d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-130">Members of a private distribution list can be any mail-enabled user, contacts or distribution lists from Active Directory, or contacts or private distribution lists from a user's Contacts folder.</span></span>
  
<span data-ttu-id="7e3bd-131">Pour des contacts ou des listes de distribution privée, les identificateurs d’élément sont retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-131">For contacts or private distribution lists, the item identifiers are returned in the response.</span></span> <span data-ttu-id="7e3bd-132">Cela peut servir à obtenir des informations sur l’objet ou de développer l’appartenance à une liste de distribution privée.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-132">This can be used to get information about the object or to expand membership in a private distribution list.</span></span>
  
## <a name="expanddl-private-distribution-list-request-example"></a><span data-ttu-id="7e3bd-133">Exemple de requête de liste de Distribution privée ExpandDL</span><span class="sxs-lookup"><span data-stu-id="7e3bd-133">ExpandDL Private Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="7e3bd-134">Description</span><span class="sxs-lookup"><span data-stu-id="7e3bd-134">Description</span></span>

<span data-ttu-id="7e3bd-135">L’exemple suivant d’une demande ExpandDL indique comment former une demande pour développer une liste de distribution privée.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-135">The following example of an ExpandDL request shows how to form a request to expand a private distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="7e3bd-136">Code</span><span class="sxs-lookup"><span data-stu-id="7e3bd-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:ItemId Id="xASUAd==" ChangeKey="AAts0Q=="/>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="7e3bd-137">Commentaires</span><span class="sxs-lookup"><span data-stu-id="7e3bd-137">Comments</span></span>

<span data-ttu-id="7e3bd-138">Pour développer une liste de distribution privée, l’élément de [boîte aux lettres](mailbox.md) contient l’élément [ItemId](itemid.md) qui identifie une liste de distribution privée dans la boîte aux lettres de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-138">To expand a private distribution list, the [Mailbox](mailbox.md) element will contain the [ItemId](itemid.md) element that identifies a private distribution list in the user's mailbox.</span></span> 
  
## <a name="expanddl-public-distribution-list-request-example"></a><span data-ttu-id="7e3bd-139">Exemple de requête de liste de Distribution publique ExpandDL</span><span class="sxs-lookup"><span data-stu-id="7e3bd-139">ExpandDL Public Distribution List request example</span></span>

### <a name="description"></a><span data-ttu-id="7e3bd-140">Description</span><span class="sxs-lookup"><span data-stu-id="7e3bd-140">Description</span></span>

<span data-ttu-id="7e3bd-141">L’exemple suivant d’une demande ExpandDL indique comment former une demande pour développer une liste de distribution publique.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-141">The following example of an ExpandDL request shows how to form a request to expand a public distribution list.</span></span> <span data-ttu-id="7e3bd-142">L’exemple illustre l’utilisation d’un nom d’affichage pour développer une liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-142">The example shows the use of a display name to expand a distribution list.</span></span>
  
### <a name="code"></a><span data-ttu-id="7e3bd-143">Code</span><span class="sxs-lookup"><span data-stu-id="7e3bd-143">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
        <t:Mailbox>
          <t:EmailAddress>TheDistributionList</t:EmailAddress>
        </t:Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="7e3bd-144">Commentaires</span><span class="sxs-lookup"><span data-stu-id="7e3bd-144">Comments</span></span>

<span data-ttu-id="7e3bd-145">La réponse à cette demande contient des éléments de **boîte aux lettres** qui identifient chaque boîte aux lettres dans la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-145">The response to this request will contain **Mailbox** elements that identify each mailbox in the distribution list.</span></span> <span data-ttu-id="7e3bd-146">Si une liste de distribution est contenue dans une liste de distribution, une extension de la liste de distribution doit être effectuée sur la liste de distribution incorporées.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-146">If a distribution list is contained within a distribution list, a separate distribution list expansion must be performed on the embedded distribution list.</span></span> <span data-ttu-id="7e3bd-147">Si la liste de distribution ne possède aucun membre ou la liste de distribution demandée n’existe pas, l’attribut **ResponseClass** contient une valeur égale à la réussite.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-147">If the distribution list has no members or the requested distribution list does not exist, the **ResponseClass** attribute will contain a value equal to Success.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="7e3bd-148">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="7e3bd-148">Request elements</span></span>

<span data-ttu-id="7e3bd-149">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="7e3bd-149">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7e3bd-150">ExpandDL</span><span class="sxs-lookup"><span data-stu-id="7e3bd-150">ExpandDL</span></span>](expanddl.md)
    
- [<span data-ttu-id="7e3bd-151">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="7e3bd-151">Mailbox</span></span>](mailbox.md)
    
- <span data-ttu-id="7e3bd-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) est utilisé pour identifier les listes de distribution publiques.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-152">[EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) is used to identify public distribution lists.</span></span> <span data-ttu-id="7e3bd-153">L’élément [ItemId](itemid.md) est utilisé pour identifier les listes de distribution privée.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-153">The [ItemId](itemid.md) element is used to identify private distribution lists.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="7e3bd-154">Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-154">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-expanddl-response-example"></a><span data-ttu-id="7e3bd-155">Exemple de réponse ExpandDL réussie</span><span class="sxs-lookup"><span data-stu-id="7e3bd-155">Successful ExpandDL response example</span></span>

### <a name="description"></a><span data-ttu-id="7e3bd-156">Description</span><span class="sxs-lookup"><span data-stu-id="7e3bd-156">Description</span></span>

<span data-ttu-id="7e3bd-157">L’exemple suivant d’une réponse ExpandDL montre une réponse à la demande décrite ci-dessus.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-157">The following example of an ExpandDL response shows a response to the request described above.</span></span> <span data-ttu-id="7e3bd-158">Le développement de listes de distribution décrit les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="7e3bd-158">The distribution list expansion describes the following:</span></span> 
  
- <span data-ttu-id="7e3bd-159">Le nombre de membres de la liste de distribution qui sont retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-159">The number of members of the distribution list that are returned in the response.</span></span>
    
- <span data-ttu-id="7e3bd-160">Si la réponse contient tous les membres de la liste de distribution.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-160">Whether the response contains all the members of the distribution list.</span></span>
    
- <span data-ttu-id="7e3bd-161">Nom de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-161">The name of the mailbox.</span></span>
    
- <span data-ttu-id="7e3bd-162">L’adresse de messagerie de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-162">The e-mail address of the mailbox.</span></span>
    
- <span data-ttu-id="7e3bd-163">Le type de routage pour la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-163">The routing type for the mailbox.</span></span>
    
- <span data-ttu-id="7e3bd-164">Le type de boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-164">The type of mailbox.</span></span>
    
> [!NOTE]
> <span data-ttu-id="7e3bd-165">Nom de la liste de distribution n’est pas inclus dans la réponse ; Par conséquent, vous devez garder une trace du nom à partir de la demande.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-165">The distribution list name is not included in the response; therefore, you must keep track of the name from the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="7e3bd-166">Code</span><span class="sxs-lookup"><span data-stu-id="7e3bd-166">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="7e3bd-167">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="7e3bd-167">Successful response elements</span></span>

<span data-ttu-id="7e3bd-168">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="7e3bd-168">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7e3bd-169">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7e3bd-169">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7e3bd-170">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="7e3bd-170">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="7e3bd-171">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7e3bd-171">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7e3bd-172">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7e3bd-172">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="7e3bd-173">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7e3bd-173">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7e3bd-174">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="7e3bd-174">DLExpansion</span></span>](dlexpansion.md)
    
- [<span data-ttu-id="7e3bd-175">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="7e3bd-175">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="7e3bd-176">Nom (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7e3bd-176">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="7e3bd-177">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="7e3bd-177">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="7e3bd-178">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="7e3bd-178">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="7e3bd-179">MailboxType</span><span class="sxs-lookup"><span data-stu-id="7e3bd-179">MailboxType</span></span>](mailboxtype.md)
    
<span data-ttu-id="7e3bd-180">Pour trouver d’autres options pour le message de réponse de l’opération ExpandDL, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-180">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="7e3bd-181">Démarrez au niveau de l’élément [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="7e3bd-181">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="expanddl-error-response"></a><span data-ttu-id="7e3bd-182">Réponse d’erreur ExpandDL</span><span class="sxs-lookup"><span data-stu-id="7e3bd-182">ExpandDL error response</span></span>

### <a name="description"></a><span data-ttu-id="7e3bd-183">Description</span><span class="sxs-lookup"><span data-stu-id="7e3bd-183">Description</span></span>

<span data-ttu-id="7e3bd-184">L’exemple suivant montre une réponse d’erreur à une demande de ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-184">The following example shows an error response to an ExpandDL request.</span></span>
  
### <a name="code"></a><span data-ttu-id="7e3bd-185">Code</span><span class="sxs-lookup"><span data-stu-id="7e3bd-185">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" 
                         MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <ExpandDLResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="7e3bd-186">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="7e3bd-186">Error response elements</span></span>

<span data-ttu-id="7e3bd-187">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="7e3bd-187">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="7e3bd-188">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7e3bd-188">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7e3bd-189">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="7e3bd-189">ExpandDLResponse</span></span>](expanddlresponse.md)
    
- [<span data-ttu-id="7e3bd-190">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7e3bd-190">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7e3bd-191">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7e3bd-191">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
    
- [<span data-ttu-id="7e3bd-192">MessageText</span><span class="sxs-lookup"><span data-stu-id="7e3bd-192">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7e3bd-193">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7e3bd-193">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7e3bd-194">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7e3bd-194">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="7e3bd-195">Pour trouver d’autres options pour le message de réponse de l’opération ExpandDL, explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="7e3bd-195">To find other options for the response message of the ExpandDL operation, explore the schema hierarchy.</span></span> <span data-ttu-id="7e3bd-196">Démarrez au niveau de l’élément [ExpandDLResponse](expanddlresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="7e3bd-196">Start at the [ExpandDLResponse](expanddlresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7e3bd-197">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7e3bd-197">See also</span></span>

- [<span data-ttu-id="7e3bd-198">Opération ResolveNames</span><span class="sxs-lookup"><span data-stu-id="7e3bd-198">ResolveNames operation</span></span>](resolvenames-operation.md)
- [<span data-ttu-id="7e3bd-199">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7e3bd-199">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

