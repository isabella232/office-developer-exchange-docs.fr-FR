---
title: Opération FindItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Trouvez des informations sur l’opération EWS FindItem.
localization_priority: Priority
ms.openlocfilehash: 499d1ee80ef323c883fa86eb125d8c037fb37d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462555"
---
# <a name="finditem-operation"></a><span data-ttu-id="68d5e-103">Opération FindItem</span><span class="sxs-lookup"><span data-stu-id="68d5e-103">FindItem operation</span></span>

<span data-ttu-id="68d5e-104">Trouvez des informations sur l’opération EWS **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="68d5e-104">Find information about the **FindItem** EWS operation.</span></span> 
  
<span data-ttu-id="68d5e-105">L’opération **FindItem** recherche les éléments qui se trouvent dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="68d5e-105">The **FindItem** operation searches for items that are located in a user's mailbox.</span></span> <span data-ttu-id="68d5e-106">Cette opération offre plusieurs façons de filtrer et de mettre en forme le mode de renvoi des résultats de la recherche à l’appelant.</span><span class="sxs-lookup"><span data-stu-id="68d5e-106">This operation provides many ways to filter and format how search results are returned to the caller.</span></span> 
  
## <a name="using-the-finditem-operation"></a><span data-ttu-id="68d5e-107">Utilisation de l’opération FindItem</span><span class="sxs-lookup"><span data-stu-id="68d5e-107">Using the FindItem operation</span></span>

<span data-ttu-id="68d5e-108">La demande d’opération **FindItem** vous permet d’effectuer des recherches dans une boîte aux lettres et de mettre en forme les données renvoyées dans une réponse de plusieurs façons.</span><span class="sxs-lookup"><span data-stu-id="68d5e-108">The **FindItem** operation request provides many ways for you to search a mailbox and format how the data is returned in a response.</span></span> <span data-ttu-id="68d5e-109">Vous pouvez spécifier ce qui suit dans une requête **FindItem** :</span><span class="sxs-lookup"><span data-stu-id="68d5e-109">You can specify the following in a **FindItem** request:</span></span> 
  
- <span data-ttu-id="68d5e-110">Indique si la recherche est une traversée partielle ou supprimée de manière récupérable.</span><span class="sxs-lookup"><span data-stu-id="68d5e-110">Whether the search is a shallow or soft-deleted traversal.</span></span> <span data-ttu-id="68d5e-111">Cette spécification est requise.</span><span class="sxs-lookup"><span data-stu-id="68d5e-111">Specifying this is required.</span></span> <span data-ttu-id="68d5e-112">Notez qu’une traversée supprimée de manière récupérable combinée à une restriction de recherche entraîne zéro élément renvoyé, même si des éléments correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="68d5e-112">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned, even if there are items that match the search criteria.</span></span>
    
- <span data-ttu-id="68d5e-113">Forme de la réponse des éléments.</span><span class="sxs-lookup"><span data-stu-id="68d5e-113">The response shape of items.</span></span> <span data-ttu-id="68d5e-114">Cela identifie les propriétés qui sont renvoyées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="68d5e-114">This identifies the properties that are returned in the response.</span></span> <span data-ttu-id="68d5e-115">Cette spécification est requise.</span><span class="sxs-lookup"><span data-stu-id="68d5e-115">Specifying this is required.</span></span>
    
- <span data-ttu-id="68d5e-116">Dossiers à partir desquels effectuer la recherche.</span><span class="sxs-lookup"><span data-stu-id="68d5e-116">The folders from which to perform the search.</span></span> <span data-ttu-id="68d5e-117">Cette spécification est requise.</span><span class="sxs-lookup"><span data-stu-id="68d5e-117">Specifying this is required.</span></span>
    
- <span data-ttu-id="68d5e-118">Le mécanisme de pagination et les types d’affichage pour retourner les données d’affichage dans les pages.</span><span class="sxs-lookup"><span data-stu-id="68d5e-118">The paging mechanism and view types for returning view data in pages.</span></span> <span data-ttu-id="68d5e-119">Cette spécification est facultative.</span><span class="sxs-lookup"><span data-stu-id="68d5e-119">Specifying this is optional.</span></span>
    
- <span data-ttu-id="68d5e-120">Options de regroupement et de tri des éléments qui sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="68d5e-120">Options for grouping and sorting the items that are returned.</span></span> <span data-ttu-id="68d5e-121">Cette spécification est facultative.</span><span class="sxs-lookup"><span data-stu-id="68d5e-121">Specifying this is optional.</span></span>
    
- <span data-ttu-id="68d5e-122">Restrictions de recherche ou chaînes de syntaxe de requête avancée (AQS) pour le filtrage des éléments qui sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="68d5e-122">Search restrictions or Advanced Query Syntax (AQS) strings for filtering the items that are returned.</span></span> <span data-ttu-id="68d5e-123">Pour plus d’informations sur l’utilisation de AQS pour les recherches d’index de contenu, voir [QueryString (String)](querystring-string.md).</span><span class="sxs-lookup"><span data-stu-id="68d5e-123">For more information about using AQS for content index searches, see [QueryString (String)](querystring-string.md).</span></span> <span data-ttu-id="68d5e-124">Cette spécification est facultative.</span><span class="sxs-lookup"><span data-stu-id="68d5e-124">Specifying this is optional.</span></span>
    
- <span data-ttu-id="68d5e-125">Ordre de tri des éléments renvoyés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="68d5e-125">The sort order for items returned in the response.</span></span> <span data-ttu-id="68d5e-126">Cette spécification est facultative.</span><span class="sxs-lookup"><span data-stu-id="68d5e-126">Specifying this is optional.</span></span>
    
<span data-ttu-id="68d5e-127">L’opération **FindItem** renvoie uniquement les premiers 512 octets de toutes les propriétés transmises en continu.</span><span class="sxs-lookup"><span data-stu-id="68d5e-127">The **FindItem** operation returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="68d5e-128">Pour Unicode, elle renvoie les premiers caractères 255 à l’aide d’une chaîne Unicode terminée par un caractère null.</span><span class="sxs-lookup"><span data-stu-id="68d5e-128">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span> <span data-ttu-id="68d5e-129">Il ne renvoie aucun des formats de corps de message ou des listes de destinataires.</span><span class="sxs-lookup"><span data-stu-id="68d5e-129">It does not return any of the message body formats or the recipient lists.</span></span> <span data-ttu-id="68d5e-130">**FindItem** renverra un résumé des destinataires.</span><span class="sxs-lookup"><span data-stu-id="68d5e-130">**FindItem** will return a recipient summary.</span></span> <span data-ttu-id="68d5e-131">Vous pouvez utiliser l' [opération GetItem](getitem-operation.md) pour obtenir les détails d’un élément.</span><span class="sxs-lookup"><span data-stu-id="68d5e-131">You can use the [GetItem operation](getitem-operation.md) to get the details of an item.</span></span> 
  
 <span data-ttu-id="68d5e-132">**FindItem** renvoie uniquement l’élément [Name (EmailAddressType)](name-emailaddresstype.md) et ne renvoie pas l’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) dans l’élément [Mailbox](mailbox.md) pour les champs suivants :</span><span class="sxs-lookup"><span data-stu-id="68d5e-132">**FindItem** returns only the [Name (EmailAddressType)](name-emailaddresstype.md) element and does not return the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element in the [Mailbox](mailbox.md) element for the following fields:</span></span> 
  
- <span data-ttu-id="68d5e-133">Champ [de](from.md) pour les messages</span><span class="sxs-lookup"><span data-stu-id="68d5e-133">The [From](from.md) field for messages</span></span> 
    
- <span data-ttu-id="68d5e-134">Champ [expéditeur](sender.md) pour les messages</span><span class="sxs-lookup"><span data-stu-id="68d5e-134">The [Sender](sender.md) field for messages</span></span> 
    
- <span data-ttu-id="68d5e-135">Champ [organisateur](organizer.md) des éléments de calendrier</span><span class="sxs-lookup"><span data-stu-id="68d5e-135">The [Organizer](organizer.md) field for calendar items</span></span> 
    
> [!NOTE]
> <span data-ttu-id="68d5e-136">L’opération **FindItem** peut renvoyer des résultats dans un élément [CalendarView](calendarview.md) .</span><span class="sxs-lookup"><span data-stu-id="68d5e-136">The **FindItem** operation can return results in a [CalendarView](calendarview.md) element.</span></span> <span data-ttu-id="68d5e-137">L’élément **CalendarView** renvoie des éléments de calendrier uniques et toutes les occurrences de réunions périodiques.</span><span class="sxs-lookup"><span data-stu-id="68d5e-137">The **CalendarView** element returns single calendar items and all occurrences of recurring meetings.</span></span> <span data-ttu-id="68d5e-138">Si un élément **CalendarView** n’est pas utilisé, les éléments de calendrier uniques et les éléments de calendrier maître périodiques sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="68d5e-138">If a **CalendarView** element is not used, single calendar items and recurring master calendar items are returned.</span></span> <span data-ttu-id="68d5e-139">Les occurrences doivent être étendues à partir de la forme de base périodique si aucun élément **CalendarView** n’est utilisé.</span><span class="sxs-lookup"><span data-stu-id="68d5e-139">The occurrences must be expanded from the recurring master if a **CalendarView** element is not used.</span></span> 
  
<span data-ttu-id="68d5e-140">L’opération **FindItem** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="68d5e-140">The **FindItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="68d5e-141">**Tableau 1. En-têtes SOAP d’opération FindItem**</span><span class="sxs-lookup"><span data-stu-id="68d5e-141">**Table 1. FindItem operation SOAP headers**</span></span>

|<span data-ttu-id="68d5e-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="68d5e-142">**Header**</span></span>|<span data-ttu-id="68d5e-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="68d5e-143">**Element**</span></span>|<span data-ttu-id="68d5e-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="68d5e-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="68d5e-145">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="68d5e-145">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="68d5e-146">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="68d5e-146">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="68d5e-147">Spécifie la résolution des valeurs de données/temps dans les réponses du serveur, soit en secondes, soit en millisecondes.</span><span class="sxs-lookup"><span data-stu-id="68d5e-147">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span> <span data-ttu-id="68d5e-148">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="68d5e-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="68d5e-149">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="68d5e-149">**Impersonation**</span></span> <br/> |[<span data-ttu-id="68d5e-150">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="68d5e-150">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="68d5e-151">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="68d5e-151">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="68d5e-152">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="68d5e-152">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="68d5e-153">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="68d5e-153">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="68d5e-154">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="68d5e-154">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="68d5e-155">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="68d5e-155">Identifies the RFC3066 culture to be used to access the mailbox.</span></span> <span data-ttu-id="68d5e-156">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="68d5e-156">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="68d5e-157">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="68d5e-157">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="68d5e-158">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="68d5e-158">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="68d5e-159">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="68d5e-159">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="68d5e-160">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="68d5e-160">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="68d5e-161">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="68d5e-161">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="68d5e-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="68d5e-162">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="68d5e-163">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="68d5e-163">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="68d5e-164">Ceci s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="68d5e-164">This is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="68d5e-165">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="68d5e-165">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="68d5e-166">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="68d5e-166">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="68d5e-167">Identifie le fuseau horaire à utiliser pour toutes les réponses du serveur.</span><span class="sxs-lookup"><span data-stu-id="68d5e-167">Identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="68d5e-168">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="68d5e-168">This is applicable to a request.</span></span>  <br/> |
   
## <a name="finditem-operation-request-example"></a><span data-ttu-id="68d5e-169">Exemple de requête d’opération FindItem</span><span class="sxs-lookup"><span data-stu-id="68d5e-169">FindItem operation request example</span></span>

<span data-ttu-id="68d5e-170">L’exemple de requête **FindItem** suivant montre comment obtenir l’identificateur d’élément défini par l’énumération **IdOnly** de l’élément [BaseShape](baseshape.md) pour les éléments qui se trouvent dans le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="68d5e-170">The following example of a **FindItem** request shows how to obtain the item identifier that is defined by the **IdOnly** enumeration of the [BaseShape](baseshape.md) element for items that are found in the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
              Traversal="Shallow">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </ItemShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="68d5e-171">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="68d5e-171">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="68d5e-172">FindItem</span><span class="sxs-lookup"><span data-stu-id="68d5e-172">FindItem</span></span>](finditem.md)
    
- [<span data-ttu-id="68d5e-173">ItemShape</span><span class="sxs-lookup"><span data-stu-id="68d5e-173">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="68d5e-174">BaseShape</span><span class="sxs-lookup"><span data-stu-id="68d5e-174">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="68d5e-175">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="68d5e-175">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="68d5e-176">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="68d5e-176">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="68d5e-177">Pour plus d’options pour un message de demande **FindItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="68d5e-177">For more options for a **FindItem** request message, explore the schema hierarchy.</span></span> <span data-ttu-id="68d5e-178">Commencez par l’élément [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="68d5e-178">Start at the [FindItem](finditem.md) element.</span></span> 
  
## <a name="successful-finditem-operation-response"></a><span data-ttu-id="68d5e-179">Réponse de l’opération FindItem réussie</span><span class="sxs-lookup"><span data-stu-id="68d5e-179">Successful FindItem operation response</span></span>

<span data-ttu-id="68d5e-180">L’exemple suivant montre une réponse réussie à la demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="68d5e-180">The following example shows a successful response to the **FindItem** request.</span></span> 
  
<span data-ttu-id="68d5e-181">Les éléments de [message](message-ex15websvcsotherref.md) représentent les messages électroniques et tous les autres éléments qui ne sont pas fortement typés par le schéma EWS.</span><span class="sxs-lookup"><span data-stu-id="68d5e-181">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the EWS schema.</span></span> <span data-ttu-id="68d5e-182">Des éléments tels que IPM. Le partage et IPM. InfoPath sont renvoyés en tant qu’éléments [message](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="68d5e-182">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="68d5e-183">Exchange ne retourne pas l’élément [élément](item.md) de base dans les réponses.</span><span class="sxs-lookup"><span data-stu-id="68d5e-183">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="10" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AS4AUn=" ChangeKey="fsVU4==" />
              </t:Message>
              <t:Message>
                <t:ItemId Id="AS4AUM=" ChangeKey="fsVUA==" />
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="68d5e-184">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="68d5e-184">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="68d5e-185">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="68d5e-185">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="68d5e-186">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="68d5e-186">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="68d5e-187">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="68d5e-187">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="68d5e-188">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="68d5e-188">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="68d5e-189">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="68d5e-189">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="68d5e-190">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="68d5e-190">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="68d5e-191">Items</span><span class="sxs-lookup"><span data-stu-id="68d5e-191">Items</span></span>](items.md)
    
- [<span data-ttu-id="68d5e-192">Message</span><span class="sxs-lookup"><span data-stu-id="68d5e-192">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="68d5e-193">ItemId</span><span class="sxs-lookup"><span data-stu-id="68d5e-193">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="68d5e-194">Pour plus d’options pour un message de réponse **FindItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="68d5e-194">For more options for a **FindItem** response message, explore the schema hierarchy.</span></span> <span data-ttu-id="68d5e-195">Commencez par l’élément [FindItemResponse](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="68d5e-195">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="finditem-operation-error-response"></a><span data-ttu-id="68d5e-196">Réponse d’erreur d’opération FindItem</span><span class="sxs-lookup"><span data-stu-id="68d5e-196">FindItem operation error response</span></span>

<span data-ttu-id="68d5e-197">L’exemple suivant montre une réponse d’erreur à une requête **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="68d5e-197">The following example shows an error response to a **FindItem** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </FindItemResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="68d5e-198">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="68d5e-198">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="68d5e-199">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="68d5e-199">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="68d5e-200">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="68d5e-200">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="68d5e-201">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="68d5e-201">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="68d5e-202">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="68d5e-202">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="68d5e-203">MessageText</span><span class="sxs-lookup"><span data-stu-id="68d5e-203">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="68d5e-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="68d5e-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="68d5e-205">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="68d5e-205">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="68d5e-206">Pour plus d’options pour un message de réponse d’erreur **FindItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="68d5e-206">For more options for a **FindItem** error response message, explore the schema hierarchy.</span></span> <span data-ttu-id="68d5e-207">Commencez par l’élément [FindItemResponse](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="68d5e-207">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="version-differences"></a><span data-ttu-id="68d5e-208">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="68d5e-208">Version differences</span></span>

<span data-ttu-id="68d5e-209">Les versions d’Exchange commençant par la version principale 15 et se terminant par Build 15.0.898.11 renvoient une valeur ErrorInvalidOperation dans l’élément [ResponseCode](responsecode.md) lorsque l’opération **FindItem** est utilisée pour rechercher plusieurs dossiers dans une boîte aux lettres d’archivage.</span><span class="sxs-lookup"><span data-stu-id="68d5e-209">Versions of Exchange starting with major version 15 and ending with build 15.0.898.11 return an ErrorInvalidOperation value in the [ResponseCode](responsecode.md) element when the **FindItem** operation is used to search multiple folders in an archive mailbox.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="68d5e-210">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="68d5e-210">See also</span></span>

- [<span data-ttu-id="68d5e-211">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="68d5e-211">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [<span data-ttu-id="68d5e-212">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="68d5e-212">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
    
- <span data-ttu-id="68d5e-213">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="68d5e-213">**FindItemType**</span></span>
    

