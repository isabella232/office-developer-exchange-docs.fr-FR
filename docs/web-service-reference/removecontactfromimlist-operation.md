---
title: Opération RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Trouvez des informations sur l’opération EWS RemoveContactFromImList.
ms.openlocfilehash: 8b3d83a0b53bad169d9f3478540e5087901f3a12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458466"
---
# <a name="removecontactfromimlist-operation"></a><span data-ttu-id="d7a85-103">Opération RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="d7a85-103">RemoveContactFromImList operation</span></span>

<span data-ttu-id="d7a85-104">Trouvez des informations sur l’opération EWS **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="d7a85-104">Find information about the **RemoveContactFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="d7a85-105">L’opération **RemoveContactFromImList** supprime les contacts de la liste de messagerie instantanée Lync lorsque Lync utilise Exchange pour le magasin de contacts.</span><span class="sxs-lookup"><span data-stu-id="d7a85-105">The **RemoveContactFromImList** operation removes contacts from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="d7a85-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d7a85-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removecontactfromimlist-operation"></a><span data-ttu-id="d7a85-107">Utilisation de l’opération RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="d7a85-107">Using the RemoveContactFromImList operation</span></span>

<span data-ttu-id="d7a85-108">L’opération **RemoveContactFromImList** accepte un seul argument qui identifie un contact à supprimer de la liste des contacts Lync stockée sur un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="d7a85-108">The **RemoveContactFromImList** operation accepts a single argument that identifies a contact to remove from the Lync contact list stored on an Exchange server.</span></span> <span data-ttu-id="d7a85-109">La liste des contacts ciblés par cette opération est appelée **contacts Lync** dans Outlook 2013.</span><span class="sxs-lookup"><span data-stu-id="d7a85-109">The list of contacts that this operation targets is called **Lync Contacts** in Outlook 2013.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="d7a85-110">N’utilisez pas l' [opération DeleteItem](deleteitem-operation.md) pour supprimer des contacts d’une liste de contacts.</span><span class="sxs-lookup"><span data-stu-id="d7a85-110">Do not use the [DeleteItem operation](deleteitem-operation.md) to remove contacts from a contact list.</span></span> <span data-ttu-id="d7a85-111">Un traitement supplémentaire côté serveur peut être nécessaire pour prendre en charge la suppression d’un contact de la liste de **contacts Lync** .</span><span class="sxs-lookup"><span data-stu-id="d7a85-111">Additional server-side processing might have to occur to support removing a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="d7a85-112">Notez que la liste de **contacts Lync** est l’équivalent conceptuel du dossier de boîte aux lettres **contacts Lync** par défaut.</span><span class="sxs-lookup"><span data-stu-id="d7a85-112">Note that the **Lync Contacts** list is the conceptual equivalent of the default **Lync Contacts** mailbox folder.</span></span> 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a><span data-ttu-id="d7a85-113">En-têtes SOAP d’opération RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="d7a85-113">RemoveContactFromImList operation SOAP headers</span></span>

<span data-ttu-id="d7a85-114">L’opération **RemoveContactFromImList** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d7a85-114">The **RemoveContactFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d7a85-115">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="d7a85-115">**Header name**</span></span>|<span data-ttu-id="d7a85-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d7a85-116">**Element**</span></span>|<span data-ttu-id="d7a85-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="d7a85-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d7a85-118">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="d7a85-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="d7a85-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="d7a85-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d7a85-120">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="d7a85-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="d7a85-121">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="d7a85-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d7a85-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="d7a85-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="d7a85-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="d7a85-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="d7a85-124">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d7a85-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="d7a85-125">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="d7a85-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d7a85-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d7a85-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d7a85-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d7a85-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d7a85-128">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="d7a85-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d7a85-129">Cet en-tête s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="d7a85-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d7a85-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d7a85-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d7a85-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d7a85-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d7a85-132">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="d7a85-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d7a85-133">Cet en-tête s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="d7a85-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a><span data-ttu-id="d7a85-134">Exemple de requête d’opération RemoveContactFromImList : supprimer un contact de la liste de contacts Lync</span><span class="sxs-lookup"><span data-stu-id="d7a85-134">RemoveContactFromImList operation request example: Remove a contact from the Lync Contacts list</span></span>

<span data-ttu-id="d7a85-135">L’exemple suivant de demande d’opération **RemoveContactFromImList** montre comment supprimer un contact de la liste de **contacts Lync** .</span><span class="sxs-lookup"><span data-stu-id="d7a85-135">The following example of a **RemoveContactFromImList** operation request shows how to remove a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="d7a85-136">L’opération **RemoveContactFromImList** accepte un seul identificateur de contact unique pour identifier le contact qui est supprimé de la liste de **contacts Lync** .</span><span class="sxs-lookup"><span data-stu-id="d7a85-136">The **RemoveContactFromImList** operation accepts a single unique contact identifier to identify the contact that is removed from the **Lync Contacts** list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d7a85-137">Tous les identificateurs d’élément et clés de modification de cet article ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="d7a85-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
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

<span data-ttu-id="d7a85-138">Les éléments suivants sont utilisés dans le corps SOAP de la demande :</span><span class="sxs-lookup"><span data-stu-id="d7a85-138">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="d7a85-139">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="d7a85-139">RemoveContactFromImList</span></span>](removecontactfromimlist.md)
    
- [<span data-ttu-id="d7a85-140">Mettez</span><span class="sxs-lookup"><span data-stu-id="d7a85-140">ContactId</span></span>](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a><span data-ttu-id="d7a85-141">Réponse de l’opération RemoveContactFromImList réussie</span><span class="sxs-lookup"><span data-stu-id="d7a85-141">Successful RemoveContactFromImList operation response</span></span>

<span data-ttu-id="d7a85-142">L’exemple suivant montre une réponse réussie à une demande d’opération **RemoveContactFromImList** pour supprimer un contact de la liste de **contacts Lync** .</span><span class="sxs-lookup"><span data-stu-id="d7a85-142">The following example shows a successful response to a **RemoveContactFromImList** operation request to remove a contact from the **Lync Contacts** list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="d7a85-143">Les éléments suivants sont utilisés dans le corps SOAP de réponse :</span><span class="sxs-lookup"><span data-stu-id="d7a85-143">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="d7a85-144">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="d7a85-144">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="d7a85-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7a85-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a><span data-ttu-id="d7a85-146">Réponse d’erreur d’opération RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="d7a85-146">RemoveContactFromImList operation error response</span></span>

<span data-ttu-id="d7a85-147">L’exemple suivant montre une réponse d’erreur à une demande d’opération **RemoveContactFromImList** .</span><span class="sxs-lookup"><span data-stu-id="d7a85-147">The following example shows an error response to a **RemoveContactFromImList** operation request.</span></span> <span data-ttu-id="d7a85-148">Réponse à une demande de suppression d’un contact de la liste de **contacts Lync** lorsque le contact n’existe plus dans la liste.</span><span class="sxs-lookup"><span data-stu-id="d7a85-148">This is a response to a request to remove a contact from the **Lync Contacts** list when the contact no longer exists in the list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="d7a85-149">Les éléments suivants sont utilisés dans le corps SOAP de la réponse d’erreur :</span><span class="sxs-lookup"><span data-stu-id="d7a85-149">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="d7a85-150">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="d7a85-150">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="d7a85-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="d7a85-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d7a85-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d7a85-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d7a85-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d7a85-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="d7a85-154">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d7a85-154">See also</span></span>

- [<span data-ttu-id="d7a85-155">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d7a85-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="d7a85-156">Opération GetImItemList</span><span class="sxs-lookup"><span data-stu-id="d7a85-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

