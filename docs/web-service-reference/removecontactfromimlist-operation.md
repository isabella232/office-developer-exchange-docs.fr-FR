---
title: Opération RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Opération de recherche plus d’informations sur la RemoveContactFromImList EWS.
ms.openlocfilehash: 036b295a84e86ad74c467572cc52fdf6bbae5191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829080"
---
# <a name="removecontactfromimlist-operation"></a><span data-ttu-id="f1823-103">Opération RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="f1823-103">RemoveContactFromImList operation</span></span>

<span data-ttu-id="f1823-104">Trouvez des informations sur l’opération EWS **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="f1823-104">Find information about the **RemoveContactFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="f1823-105">L’opération **RemoveContactFromImList** supprime les contacts de la liste de la messagerie instantanée (MI) de Lync lorsque Lync utilise Exchange pour le magasin de contacts.</span><span class="sxs-lookup"><span data-stu-id="f1823-105">The **RemoveContactFromImList** operation removes contacts from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="f1823-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f1823-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removecontactfromimlist-operation"></a><span data-ttu-id="f1823-107">Utilisation de l’opération RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="f1823-107">Using the RemoveContactFromImList operation</span></span>

<span data-ttu-id="f1823-108">L’opération **RemoveContactFromImList** accepte un argument unique qui identifie un contact à supprimer de la liste des contacts Lync stockée sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="f1823-108">The **RemoveContactFromImList** operation accepts a single argument that identifies a contact to remove from the Lync contact list stored on an Exchange server.</span></span> <span data-ttu-id="f1823-109">La liste des contacts que les objectifs de cette opération est appelée **Contacts Lync** dans Outlook 2013.</span><span class="sxs-lookup"><span data-stu-id="f1823-109">The list of contacts that this operation targets is called **Lync Contacts** in Outlook 2013.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="f1823-110">N’utilisez pas l' [opération DeleteItem](deleteitem-operation.md) pour supprimer des contacts à partir d’une liste de contacts.</span><span class="sxs-lookup"><span data-stu-id="f1823-110">Do not use the [DeleteItem operation](deleteitem-operation.md) to remove contacts from a contact list.</span></span> <span data-ttu-id="f1823-111">Traitement côté serveur supplémentaire devront se produisent pour prendre en charge la suppression d’un contact dans la liste de **Contacts Lync** .</span><span class="sxs-lookup"><span data-stu-id="f1823-111">Additional server-side processing might have to occur to support removing a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="f1823-112">Notez que la liste de **Contacts Lync** est l’équivalent conceptuelle du dossier par défaut **Contacts Lync** boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f1823-112">Note that the **Lync Contacts** list is the conceptual equivalent of the default **Lync Contacts** mailbox folder.</span></span> 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a><span data-ttu-id="f1823-113">En-têtes SOAP RemoveContactFromImList opération</span><span class="sxs-lookup"><span data-stu-id="f1823-113">RemoveContactFromImList operation SOAP headers</span></span>

<span data-ttu-id="f1823-114">L’opération **RemoveContactFromImList** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="f1823-114">The **RemoveContactFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="f1823-115">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="f1823-115">**Header name**</span></span>|<span data-ttu-id="f1823-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f1823-116">**Element**</span></span>|<span data-ttu-id="f1823-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="f1823-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f1823-118">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="f1823-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="f1823-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="f1823-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="f1823-120">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="f1823-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="f1823-121">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="f1823-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f1823-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="f1823-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="f1823-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="f1823-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="f1823-124">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="f1823-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="f1823-125">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="f1823-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f1823-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="f1823-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="f1823-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="f1823-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="f1823-128">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="f1823-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="f1823-129">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="f1823-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f1823-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="f1823-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="f1823-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f1823-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="f1823-132">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="f1823-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="f1823-133">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="f1823-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a><span data-ttu-id="f1823-134">Exemple de requête d’opération RemoveContactFromImList : supprimer un contact de la liste de Contacts Lync</span><span class="sxs-lookup"><span data-stu-id="f1823-134">RemoveContactFromImList operation request example: Remove a contact from the Lync Contacts list</span></span>

<span data-ttu-id="f1823-135">Une demande d’opération **RemoveContactFromImList** l’exemple suivant montre comment supprimer un contact de la liste de **Contacts Lync** .</span><span class="sxs-lookup"><span data-stu-id="f1823-135">The following example of a **RemoveContactFromImList** operation request shows how to remove a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="f1823-136">L’opération **RemoveContactFromImList** accepte un identificateur contact unique pour identifier le contact est supprimé de la liste de **Contacts Lync** .</span><span class="sxs-lookup"><span data-stu-id="f1823-136">The **RemoveContactFromImList** operation accepts a single unique contact identifier to identify the contact that is removed from the **Lync Contacts** list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f1823-137">Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="f1823-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="f1823-138">Les éléments suivants sont utilisés dans la demande SOAP body :</span><span class="sxs-lookup"><span data-stu-id="f1823-138">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="f1823-139">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="f1823-139">RemoveContactFromImList</span></span>](removecontactfromimlist.md)
    
- [<span data-ttu-id="f1823-140">ContactId</span><span class="sxs-lookup"><span data-stu-id="f1823-140">ContactId</span></span>](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a><span data-ttu-id="f1823-141">Réponse d’opération RemoveContactFromImList réussie</span><span class="sxs-lookup"><span data-stu-id="f1823-141">Successful RemoveContactFromImList operation response</span></span>

<span data-ttu-id="f1823-142">L’exemple suivant montre une réponse positive à une demande d’opération **RemoveContactFromImList** pour supprimer un contact dans la liste de **Contacts Lync** .</span><span class="sxs-lookup"><span data-stu-id="f1823-142">The following example shows a successful response to a **RemoveContactFromImList** operation request to remove a contact from the **Lync Contacts** list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="f1823-143">Les éléments suivants sont utilisés dans la réponse SOAP body :</span><span class="sxs-lookup"><span data-stu-id="f1823-143">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="f1823-144">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="f1823-144">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="f1823-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f1823-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a><span data-ttu-id="f1823-146">Réponse d’erreur d’opération RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="f1823-146">RemoveContactFromImList operation error response</span></span>

<span data-ttu-id="f1823-147">L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="f1823-147">The following example shows an error response to a **RemoveContactFromImList** operation request.</span></span> <span data-ttu-id="f1823-148">Il s’agit d’une réponse à une demande pour supprimer un contact dans la liste de **Contacts Lync** lorsque le contact n’existe plus dans la liste.</span><span class="sxs-lookup"><span data-stu-id="f1823-148">This is a response to a request to remove a contact from the **Lync Contacts** list when the contact no longer exists in the list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="f1823-149">Les éléments suivants sont utilisés dans le corps SOAP de la réponse d’erreur :</span><span class="sxs-lookup"><span data-stu-id="f1823-149">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="f1823-150">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="f1823-150">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="f1823-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="f1823-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f1823-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f1823-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f1823-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f1823-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="f1823-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f1823-154">See also</span></span>

- [<span data-ttu-id="f1823-155">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f1823-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="f1823-156">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="f1823-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

