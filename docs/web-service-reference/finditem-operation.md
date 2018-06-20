---
title: FindItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItem
api_type:
- schema
ms.assetid: ebad6aae-16e7-44de-ae63-a95b24539729
description: Opération de recherche plus d’informations sur la EWS FindItem.
ms.openlocfilehash: b033ac2930981819a20f1336d40058a5f7c03b89
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756405"
---
# <a name="finditem-operation"></a><span data-ttu-id="50e0f-103">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="50e0f-103">FindItem operation</span></span>

<span data-ttu-id="50e0f-104">Trouvez des informations sur l’opération EWS **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="50e0f-104">Find information about the **FindItem** EWS operation.</span></span> 
  
<span data-ttu-id="50e0f-105">L’opération **FindItem** recherche des éléments qui sont trouvent dans la boîte aux lettres d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="50e0f-105">The **FindItem** operation searches for items that are located in a user's mailbox.</span></span> <span data-ttu-id="50e0f-106">Cette opération fournit de nombreuses façons de filtrer et comment les résultats de la recherche sont renvoyés à l’appelant de format.</span><span class="sxs-lookup"><span data-stu-id="50e0f-106">This operation provides many ways to filter and format how search results are returned to the caller.</span></span> 
  
## <a name="using-the-finditem-operation"></a><span data-ttu-id="50e0f-107">Utilisation de l’opération FindItem</span><span class="sxs-lookup"><span data-stu-id="50e0f-107">Using the FindItem operation</span></span>

<span data-ttu-id="50e0f-108">La requête d’opération **FindItem** offre de nombreux moyens pour rechercher une boîte aux lettres et le format comment les données sont retournées dans une réponse.</span><span class="sxs-lookup"><span data-stu-id="50e0f-108">The **FindItem** operation request provides many ways for you to search a mailbox and format how the data is returned in a response.</span></span> <span data-ttu-id="50e0f-109">Vous pouvez spécifier ce qui suit dans une requête **FindItem** :</span><span class="sxs-lookup"><span data-stu-id="50e0f-109">You can specify the following in a **FindItem** request:</span></span> 
  
- <span data-ttu-id="50e0f-110">Si la recherche est un parcours superficiel ou supprimée.</span><span class="sxs-lookup"><span data-stu-id="50e0f-110">Whether the search is a shallow or soft-deleted traversal.</span></span> <span data-ttu-id="50e0f-111">Cette spécification est requis.</span><span class="sxs-lookup"><span data-stu-id="50e0f-111">Specifying this is required.</span></span> <span data-ttu-id="50e0f-112">Notez qu’un parcours récupérable combiné à une restriction de recherche entraînera zéro éléments retournés, même s’il existe des éléments qui correspondent aux critères de recherche.</span><span class="sxs-lookup"><span data-stu-id="50e0f-112">Note that a soft-deleted traversal combined with a search restriction will result in zero items returned, even if there are items that match the search criteria.</span></span>
    
- <span data-ttu-id="50e0f-113">La forme de réponse d’éléments.</span><span class="sxs-lookup"><span data-stu-id="50e0f-113">The response shape of items.</span></span> <span data-ttu-id="50e0f-114">Ces informations identifient les propriétés qui sont retournées dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="50e0f-114">This identifies the properties that are returned in the response.</span></span> <span data-ttu-id="50e0f-115">Cette spécification est requis.</span><span class="sxs-lookup"><span data-stu-id="50e0f-115">Specifying this is required.</span></span>
    
- <span data-ttu-id="50e0f-116">Les dossiers à partir de laquelle effectuer la recherche.</span><span class="sxs-lookup"><span data-stu-id="50e0f-116">The folders from which to perform the search.</span></span> <span data-ttu-id="50e0f-117">Cette spécification est requis.</span><span class="sxs-lookup"><span data-stu-id="50e0f-117">Specifying this is required.</span></span>
    
- <span data-ttu-id="50e0f-118">Les types de mécanisme et affichage de pagination pour le renvoi d’afficher des données dans les pages.</span><span class="sxs-lookup"><span data-stu-id="50e0f-118">The paging mechanism and view types for returning view data in pages.</span></span> <span data-ttu-id="50e0f-119">Cette spécification est facultative.</span><span class="sxs-lookup"><span data-stu-id="50e0f-119">Specifying this is optional.</span></span>
    
- <span data-ttu-id="50e0f-120">Options de regroupement et de tri des éléments qui sont retournés.</span><span class="sxs-lookup"><span data-stu-id="50e0f-120">Options for grouping and sorting the items that are returned.</span></span> <span data-ttu-id="50e0f-121">Cette spécification est facultative.</span><span class="sxs-lookup"><span data-stu-id="50e0f-121">Specifying this is optional.</span></span>
    
- <span data-ttu-id="50e0f-122">Restrictions de recherche ou des chaînes de syntaxe de requête avancée (AQS) pour filtrer les éléments qui sont retournés.</span><span class="sxs-lookup"><span data-stu-id="50e0f-122">Search restrictions or Advanced Query Syntax (AQS) strings for filtering the items that are returned.</span></span> <span data-ttu-id="50e0f-123">Pour plus d’informations sur l’utilisation de AQS pour les recherches de l’index de contenu, voir [QueryString (chaîne)](querystring-string.md).</span><span class="sxs-lookup"><span data-stu-id="50e0f-123">For more information about using AQS for content index searches, see [QueryString (String)](querystring-string.md).</span></span> <span data-ttu-id="50e0f-124">Cette spécification est facultative.</span><span class="sxs-lookup"><span data-stu-id="50e0f-124">Specifying this is optional.</span></span>
    
- <span data-ttu-id="50e0f-125">L’ordre de tri des éléments retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="50e0f-125">The sort order for items returned in the response.</span></span> <span data-ttu-id="50e0f-126">Cette spécification est facultative.</span><span class="sxs-lookup"><span data-stu-id="50e0f-126">Specifying this is optional.</span></span>
    
<span data-ttu-id="50e0f-127">L’opération **FindItem** renvoie uniquement les 512 octets de n’importe quelle propriété lisible en continu.</span><span class="sxs-lookup"><span data-stu-id="50e0f-127">The **FindItem** operation returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="50e0f-128">Pour le format Unicode, elle renvoie les 255 premiers caractères à l’aide d’une chaîne Unicode terminée par null.</span><span class="sxs-lookup"><span data-stu-id="50e0f-128">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span> <span data-ttu-id="50e0f-129">Elle ne renvoie pas les formats de corps de message ou les listes de destinataires.</span><span class="sxs-lookup"><span data-stu-id="50e0f-129">It does not return any of the message body formats or the recipient lists.</span></span> <span data-ttu-id="50e0f-130">**FindItem** renverra un destinataire résumé.</span><span class="sxs-lookup"><span data-stu-id="50e0f-130">**FindItem** will return a recipient summary.</span></span> <span data-ttu-id="50e0f-131">Vous pouvez utiliser l' [opération GetItem](getitem-operation.md) pour obtenir les détails d’un élément.</span><span class="sxs-lookup"><span data-stu-id="50e0f-131">You can use the [GetItem operation](getitem-operation.md) to get the details of an item.</span></span> 
  
 <span data-ttu-id="50e0f-132">**FindItem** renvoie uniquement l’élément [nom (EmailAddressType)](name-emailaddresstype.md) et ne retourne pas l’élément [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) dans l’élément de [boîte aux lettres](mailbox.md) pour les champs suivants :</span><span class="sxs-lookup"><span data-stu-id="50e0f-132">**FindItem** returns only the [Name (EmailAddressType)](name-emailaddresstype.md) element and does not return the [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element in the [Mailbox](mailbox.md) element for the following fields:</span></span> 
  
- <span data-ttu-id="50e0f-133">Le champ [](from.md) des messages</span><span class="sxs-lookup"><span data-stu-id="50e0f-133">The [From](from.md) field for messages</span></span> 
    
- <span data-ttu-id="50e0f-134">Le champ de [l’expéditeur](sender.md) pour les messages</span><span class="sxs-lookup"><span data-stu-id="50e0f-134">The [Sender](sender.md) field for messages</span></span> 
    
- <span data-ttu-id="50e0f-135">Le champ [organisateur](organizer.md) des éléments de calendrier</span><span class="sxs-lookup"><span data-stu-id="50e0f-135">The [Organizer](organizer.md) field for calendar items</span></span> 
    
> [!NOTE]
> <span data-ttu-id="50e0f-136">L’opération **FindItem** peut retourner des résultats dans un élément [CalendarView](calendarview.md) .</span><span class="sxs-lookup"><span data-stu-id="50e0f-136">The **FindItem** operation can return results in a [CalendarView](calendarview.md) element.</span></span> <span data-ttu-id="50e0f-137">L’élément **CalendarView** renvoie les éléments de calendrier unique et toutes les occurrences des réunions périodiques.</span><span class="sxs-lookup"><span data-stu-id="50e0f-137">The **CalendarView** element returns single calendar items and all occurrences of recurring meetings.</span></span> <span data-ttu-id="50e0f-138">Si un élément **CalendarView** n’est pas utilisé, les éléments de calendrier et les éléments de calendrier principal périodiques sont renvoyés.</span><span class="sxs-lookup"><span data-stu-id="50e0f-138">If a **CalendarView** element is not used, single calendar items and recurring master calendar items are returned.</span></span> <span data-ttu-id="50e0f-139">Si un élément **CalendarView** n’est pas utilisé, les occurrences doivent être développées à partir de la forme de base périodique.</span><span class="sxs-lookup"><span data-stu-id="50e0f-139">The occurrences must be expanded from the recurring master if a **CalendarView** element is not used.</span></span> 
  
<span data-ttu-id="50e0f-140">L’opération **FindItem** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="50e0f-140">The **FindItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="50e0f-141">**Le tableau 1. En-têtes SOAP FindItem opération**</span><span class="sxs-lookup"><span data-stu-id="50e0f-141">**Table 1. FindItem operation SOAP headers**</span></span>

|<span data-ttu-id="50e0f-142">**Header**</span><span class="sxs-lookup"><span data-stu-id="50e0f-142">**Header**</span></span>|<span data-ttu-id="50e0f-143">**Élément**</span><span class="sxs-lookup"><span data-stu-id="50e0f-143">**Element**</span></span>|<span data-ttu-id="50e0f-144">**Description**</span><span class="sxs-lookup"><span data-stu-id="50e0f-144">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="50e0f-145">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="50e0f-145">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="50e0f-146">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="50e0f-146">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="50e0f-147">Spécifie la résolution des valeurs de date/heure dans les réponses à partir du serveur, en secondes ou en millisecondes.</span><span class="sxs-lookup"><span data-stu-id="50e0f-147">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span> <span data-ttu-id="50e0f-148">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="50e0f-148">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="50e0f-149">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="50e0f-149">**Impersonation**</span></span> <br/> |[<span data-ttu-id="50e0f-150">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="50e0f-150">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="50e0f-151">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="50e0f-151">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="50e0f-152">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="50e0f-152">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="50e0f-153">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="50e0f-153">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="50e0f-154">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="50e0f-154">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="50e0f-155">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="50e0f-155">Identifies the RFC3066 culture to be used to access the mailbox.</span></span> <span data-ttu-id="50e0f-156">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="50e0f-156">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="50e0f-157">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="50e0f-157">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="50e0f-158">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="50e0f-158">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="50e0f-159">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="50e0f-159">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="50e0f-160">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="50e0f-160">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="50e0f-161">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="50e0f-161">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="50e0f-162">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="50e0f-162">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="50e0f-163">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="50e0f-163">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="50e0f-164">Cela s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="50e0f-164">This is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="50e0f-165">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="50e0f-165">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="50e0f-166">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="50e0f-166">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="50e0f-167">Identifie le fuseau horaire à utiliser pour toutes les réponses à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="50e0f-167">Identifies the time zone to be used for all responses from the server.</span></span> <span data-ttu-id="50e0f-168">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="50e0f-168">This is applicable to a request.</span></span>  <br/> |
   
## <a name="finditem-operation-request-example"></a><span data-ttu-id="50e0f-169">Exemple de requête d’opération FindItem</span><span class="sxs-lookup"><span data-stu-id="50e0f-169">FindItem operation request example</span></span>

<span data-ttu-id="50e0f-170">Une demande **FindItem** l’exemple suivant montre comment obtenir l’identificateur d’élément qui est définie par l’énumération **IdOnly** de l’élément [BaseShape](baseshape.md) pour les éléments qui se trouvent dans le dossier éléments supprimés.</span><span class="sxs-lookup"><span data-stu-id="50e0f-170">The following example of a **FindItem** request shows how to obtain the item identifier that is defined by the **IdOnly** enumeration of the [BaseShape](baseshape.md) element for items that are found in the Deleted Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
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

<span data-ttu-id="50e0f-171">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="50e0f-171">The following elements are used in the request:</span></span> 
  
- [<span data-ttu-id="50e0f-172">FindItem</span><span class="sxs-lookup"><span data-stu-id="50e0f-172">FindItem</span></span>](finditem.md)
    
- [<span data-ttu-id="50e0f-173">ItemShape</span><span class="sxs-lookup"><span data-stu-id="50e0f-173">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="50e0f-174">BaseShape</span><span class="sxs-lookup"><span data-stu-id="50e0f-174">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="50e0f-175">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="50e0f-175">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="50e0f-176">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="50e0f-176">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="50e0f-177">Pour plus d’options pour un message de demande **FindItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="50e0f-177">For more options for a **FindItem** request message, explore the schema hierarchy.</span></span> <span data-ttu-id="50e0f-178">Commencer à l’élément [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="50e0f-178">Start at the [FindItem](finditem.md) element.</span></span> 
  
## <a name="successful-finditem-operation-response"></a><span data-ttu-id="50e0f-179">Réponse d’opération FindItem réussie</span><span class="sxs-lookup"><span data-stu-id="50e0f-179">Successful FindItem operation response</span></span>

<span data-ttu-id="50e0f-180">L’exemple suivant montre une réponse positive à la demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="50e0f-180">The following example shows a successful response to the **FindItem** request.</span></span> 
  
<span data-ttu-id="50e0f-181">Éléments de [message](message-ex15websvcsotherref.md) représentent des messages électroniques et tous les autres éléments qui ne sont pas fortement typées dans le schéma EWS.</span><span class="sxs-lookup"><span data-stu-id="50e0f-181">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the EWS schema.</span></span> <span data-ttu-id="50e0f-182">Éléments tels que IPM. Partage et IPM.InfoPath sont renvoyés en tant qu’éléments du [Message](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="50e0f-182">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="50e0f-183">Exchange ne renvoie pas de [l’élément de base](item.md) des réponses.</span><span class="sxs-lookup"><span data-stu-id="50e0f-183">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="50e0f-184">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="50e0f-184">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="50e0f-185">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="50e0f-185">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="50e0f-186">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="50e0f-186">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="50e0f-187">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="50e0f-187">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="50e0f-188">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="50e0f-188">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="50e0f-189">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="50e0f-189">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="50e0f-190">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="50e0f-190">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="50e0f-191">Items</span><span class="sxs-lookup"><span data-stu-id="50e0f-191">Items</span></span>](items.md)
    
- [<span data-ttu-id="50e0f-192">Message</span><span class="sxs-lookup"><span data-stu-id="50e0f-192">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="50e0f-193">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="50e0f-193">ItemId</span></span>](itemid.md)
    
<span data-ttu-id="50e0f-194">Pour plus d’options pour un message de réponse **FindItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="50e0f-194">For more options for a **FindItem** response message, explore the schema hierarchy.</span></span> <span data-ttu-id="50e0f-195">Démarrez au niveau de l’élément [FindItemResponse](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="50e0f-195">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="finditem-operation-error-response"></a><span data-ttu-id="50e0f-196">Réponse d’erreur FindItem opération</span><span class="sxs-lookup"><span data-stu-id="50e0f-196">FindItem operation error response</span></span>

<span data-ttu-id="50e0f-197">L’exemple suivant montre une réponse d’erreur à une demande **FindItem** .</span><span class="sxs-lookup"><span data-stu-id="50e0f-197">The following example shows an error response to a **FindItem** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="50e0f-198">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="50e0f-198">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="50e0f-199">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="50e0f-199">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="50e0f-200">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="50e0f-200">FindItemResponse</span></span>](finditemresponse.md)
    
- [<span data-ttu-id="50e0f-201">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="50e0f-201">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="50e0f-202">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="50e0f-202">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
    
- [<span data-ttu-id="50e0f-203">MessageText</span><span class="sxs-lookup"><span data-stu-id="50e0f-203">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="50e0f-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="50e0f-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="50e0f-205">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="50e0f-205">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="50e0f-206">Pour plus d’options pour un message de réponse d’erreur **FindItem** , explorez la hiérarchie de schéma.</span><span class="sxs-lookup"><span data-stu-id="50e0f-206">For more options for a **FindItem** error response message, explore the schema hierarchy.</span></span> <span data-ttu-id="50e0f-207">Démarrez au niveau de l’élément [FindItemResponse](finditemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="50e0f-207">Start at the [FindItemResponse](finditemresponse.md) element.</span></span> 
  
## <a name="version-differences"></a><span data-ttu-id="50e0f-208">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="50e0f-208">Version differences</span></span>

<span data-ttu-id="50e0f-209">Versions d’Exchange depuis la version majeure 15 et se terminant par créer 15.0.898.11 retour une valeur ErrorInvalidOperation dans l’élément [ResponseCode](responsecode.md) lors de l’opération **FindItem** est utilisée pour rechercher plusieurs dossiers dans une boîte aux lettres d’archive.</span><span class="sxs-lookup"><span data-stu-id="50e0f-209">Versions of Exchange starting with major version 15 and ending with build 15.0.898.11 return an ErrorInvalidOperation value in the [ResponseCode](responsecode.md) element when the **FindItem** operation is used to search multiple folders in an archive mailbox.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="50e0f-210">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="50e0f-210">See also</span></span>

- [<span data-ttu-id="50e0f-211">Recherche d’éléments</span><span class="sxs-lookup"><span data-stu-id="50e0f-211">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)
    
- [<span data-ttu-id="50e0f-212">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="50e0f-212">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
    
- <span data-ttu-id="50e0f-213">**FindItemType**</span><span class="sxs-lookup"><span data-stu-id="50e0f-213">**FindItemType**</span></span>
    

