---
title: Opération FindFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolder
api_type:
- schema
ms.assetid: 7a9855aa-06cc-45ba-ad2a-645c15b7d031
description: L’opération FindFolder utilise les services Web Exchange pour rechercher des sous-dossiers d’un dossier identifié et renvoie un ensemble de propriétés qui décrivent le jeu de sous-dossiers.
ms.openlocfilehash: f1cc199bdaf684d8d74687ed7f064eb66fee48ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462583"
---
# <a name="findfolder-operation"></a><span data-ttu-id="ae344-103">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="ae344-103">FindFolder operation</span></span>

<span data-ttu-id="ae344-104">L’opération **FindFolder** utilise les services Web Exchange pour rechercher des sous-dossiers d’un dossier identifié et renvoie un ensemble de propriétés qui décrivent le jeu de sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="ae344-104">The **FindFolder** operation uses Exchange Web Services to find subfolders of an identified folder and returns a set of properties that describe the set of subfolders.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ae344-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="ae344-105">Remarks</span></span>

<span data-ttu-id="ae344-106">FindFolder renvoie uniquement les premiers 512 octets de toutes les propriétés transmises en continu.</span><span class="sxs-lookup"><span data-stu-id="ae344-106">FindFolder returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="ae344-107">Pour Unicode, elle renvoie les premiers caractères 255 à l’aide d’une chaîne Unicode terminée par un caractère null.</span><span class="sxs-lookup"><span data-stu-id="ae344-107">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span>
  
<span data-ttu-id="ae344-108">Les requêtes de parcours approfondi ne peuvent pas être exécutées sur les dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="ae344-108">Deep traversal queries cannot be performed on public folders.</span></span>
  
<span data-ttu-id="ae344-109">Les restrictions sont autorisées et doivent utiliser uniquement les propriétés du dossier, pas les propriétés de l’élément.</span><span class="sxs-lookup"><span data-stu-id="ae344-109">Restrictions are permitted and should use only the folder properties, not the item properties.</span></span> <span data-ttu-id="ae344-110">La fonctionnalité de tri n’est pas disponible pour les réponses **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="ae344-110">Sorting functionality is not available for **FindFolder** responses.</span></span> <span data-ttu-id="ae344-111">Les requêtes regroupées ne sont pas disponibles pour les requêtes **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="ae344-111">Grouped queries are not available for **FindFolder** queries.</span></span> 
  
 <span data-ttu-id="ae344-112">**Note** L’opération **FindFolder** est également utilisée pour rechercher des dossiers gérés.</span><span class="sxs-lookup"><span data-stu-id="ae344-112">**Note** The **FindFolder** operation is also used to find managed folders.</span></span> 
  
### <a name="soap-headers"></a><span data-ttu-id="ae344-113">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="ae344-113">SOAP Headers</span></span>

<span data-ttu-id="ae344-114">L’opération **FindFolder** peut utiliser les en-têtes SOAP répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="ae344-114">The **FindFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="ae344-115">**Header**</span><span class="sxs-lookup"><span data-stu-id="ae344-115">**Header**</span></span>|<span data-ttu-id="ae344-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ae344-116">**Element**</span></span>|<span data-ttu-id="ae344-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="ae344-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ae344-118">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="ae344-118">Impersonation</span></span>  <br/> |[<span data-ttu-id="ae344-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ae344-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ae344-120">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="ae344-120">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="ae344-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ae344-121">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="ae344-122">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ae344-122">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="ae344-123">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ae344-123">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="ae344-124">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="ae344-124">RequestVersion</span></span>  <br/> |[<span data-ttu-id="ae344-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ae344-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ae344-126">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="ae344-126">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="ae344-127">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="ae344-127">ServerVersion</span></span>  <br/> |[<span data-ttu-id="ae344-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ae344-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ae344-129">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="ae344-129">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="ae344-130">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="ae344-130">TimeZoneContext</span></span>  <br/> |[<span data-ttu-id="ae344-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="ae344-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="ae344-132">Identifie le fuseau horaire à utiliser pour toutes les réponses du serveur.</span><span class="sxs-lookup"><span data-stu-id="ae344-132">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="findfolder-request-example"></a><span data-ttu-id="ae344-133">Exemple de requête FindFolder</span><span class="sxs-lookup"><span data-stu-id="ae344-133">FindFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="ae344-134">Description</span><span class="sxs-lookup"><span data-stu-id="ae344-134">Description</span></span>

<span data-ttu-id="ae344-135">L’exemple de requête **FindFolder** suivant montre comment créer une requête pour rechercher tous les dossiers situés dans une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="ae344-135">The following example of a **FindFolder** request shows how to form a request to find all the folders located in an Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ae344-136">Code</span><span class="sxs-lookup"><span data-stu-id="ae344-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ae344-137">Commentaires</span><span class="sxs-lookup"><span data-stu-id="ae344-137">Comments</span></span>

<span data-ttu-id="ae344-138">À l’aide de la valeur par défaut de l' [BaseShape](baseshape.md), la réponse renvoie le nom du dossier, l’ID du dossier, le nombre de sous-dossiers, le nombre de dossiers enfants trouvés dans le dossier et le nombre d’éléments non lus.</span><span class="sxs-lookup"><span data-stu-id="ae344-138">Using the Default value for the [BaseShape](baseshape.md), the response returns the folder name, the folder ID, the number of subfolders, the number of child folders found in the folder, and the count of unread items.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="ae344-139">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="ae344-139">Request elements</span></span>

<span data-ttu-id="ae344-140">Cette requête **FindFolder** inclut les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ae344-140">This **FindFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="ae344-141">FindFolder</span><span class="sxs-lookup"><span data-stu-id="ae344-141">FindFolder</span></span>](findfolder.md)
    
- [<span data-ttu-id="ae344-142">FolderShape</span><span class="sxs-lookup"><span data-stu-id="ae344-142">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="ae344-143">BaseShape</span><span class="sxs-lookup"><span data-stu-id="ae344-143">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="ae344-144">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="ae344-144">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="ae344-145">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="ae344-145">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
 <span data-ttu-id="ae344-146">Pour d’autres éléments de requête **FindFolder** , voir le schéma.</span><span class="sxs-lookup"><span data-stu-id="ae344-146">For additional **FindFolder** request elements, see the schema.</span></span> 
  
## <a name="findfolder-response-example"></a><span data-ttu-id="ae344-147">Exemple de réponse FindFolder</span><span class="sxs-lookup"><span data-stu-id="ae344-147">FindFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="ae344-148">Description</span><span class="sxs-lookup"><span data-stu-id="ae344-148">Description</span></span>

<span data-ttu-id="ae344-149">L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="ae344-149">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **FindFolder** request.</span></span> <span data-ttu-id="ae344-150">La réponse contient les éléments qui sont renvoyés lorsque la valeur par défaut de l' [BaseShape](baseshape.md) est utilisée.</span><span class="sxs-lookup"><span data-stu-id="ae344-150">The response contains the elements that are returned when the Default value for the [BaseShape](baseshape.md) is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ae344-151">L’ID de dossier et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="ae344-151">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ae344-152">Code</span><span class="sxs-lookup"><span data-stu-id="ae344-152">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Folders>
              <t:Folder>
                <t:FolderId Id="AQAnAH" ChangeKey="AQAAABY" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="ae344-153">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="ae344-153">Response elements</span></span>

<span data-ttu-id="ae344-154">Les propriétés qui sont renvoyées dans la réponse sont déterminées par le [BaseShape](baseshape.md) et le [AdditionalProperties](additionalproperties.md) s’ils sont utilisés.</span><span class="sxs-lookup"><span data-stu-id="ae344-154">The properties that are returned in the response are determined by the [BaseShape](baseshape.md) and the [AdditionalProperties](additionalproperties.md) if they are used.</span></span> <span data-ttu-id="ae344-155">Une réponse **FindFolder** réussie inclut les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ae344-155">A successful **FindFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="ae344-156">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ae344-156">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ae344-157">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ae344-157">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="ae344-158">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ae344-158">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ae344-159">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ae344-159">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
    
- [<span data-ttu-id="ae344-160">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ae344-160">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ae344-161">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="ae344-161">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="ae344-162">Dossiers</span><span class="sxs-lookup"><span data-stu-id="ae344-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ae344-163">Folder</span><span class="sxs-lookup"><span data-stu-id="ae344-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="ae344-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="ae344-164">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="ae344-165">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="ae344-165">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="ae344-166">TotalCount</span><span class="sxs-lookup"><span data-stu-id="ae344-166">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="ae344-167">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="ae344-167">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="ae344-168">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="ae344-168">UnreadCount</span></span>](unreadcount.md)
    
### <a name="comments"></a><span data-ttu-id="ae344-169">Commentaires</span><span class="sxs-lookup"><span data-stu-id="ae344-169">Comments</span></span>

 <span data-ttu-id="ae344-170">**FindFolder** les réponses à une requête avec la forme de réponse **AllProperties** ne renvoient pas les éléments [totalCount](totalcount.md) et [UnreadCount](unreadcount.md) pour les recherches de dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="ae344-170">**FindFolder** responses to a request with the **AllProperties** response shape will not return the [TotalCount](totalcount.md) and [UnreadCount](unreadcount.md) elements for public folder searches.</span></span> 
  
## <a name="findfolder-error-response-example"></a><span data-ttu-id="ae344-171">Exemple de réponse d’erreur FindFolder</span><span class="sxs-lookup"><span data-stu-id="ae344-171">FindFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ae344-172">Description</span><span class="sxs-lookup"><span data-stu-id="ae344-172">Description</span></span>

<span data-ttu-id="ae344-173">L’exemple de corps SOAP suivant montre une réponse d’erreur qui se produit lorsque vous recherchez un dossier identifié par un identificateur de dossier incorrect.</span><span class="sxs-lookup"><span data-stu-id="ae344-173">The following SOAP body example shows an error response that occurs when you search for a folder that is identified by a malformed folder identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="ae344-174">Code</span><span class="sxs-lookup"><span data-stu-id="ae344-174">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </FindFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="ae344-175">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="ae344-175">Error response elements</span></span>

<span data-ttu-id="ae344-176">La réponse d’erreur **FindFolder** comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="ae344-176">The **FindFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="ae344-177">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ae344-177">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="ae344-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ae344-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ae344-179">MessageText</span><span class="sxs-lookup"><span data-stu-id="ae344-179">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ae344-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ae344-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ae344-181">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ae344-181">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="additional-information"></a><span data-ttu-id="ae344-182">Informations complémentaires</span><span class="sxs-lookup"><span data-stu-id="ae344-182">Additional Information</span></span>

- <span data-ttu-id="ae344-183">L’élément Folder [DisplayName (String)](displayname-string.md) est toujours inclus dans la forme par défaut.</span><span class="sxs-lookup"><span data-stu-id="ae344-183">The folder [DisplayName (string)](displayname-string.md) element is always included in the default shape.</span></span> 
    
- <span data-ttu-id="ae344-184">L’élément [UnreadCount](unreadcount.md) est inclus dans les dossiers tâches et notes.</span><span class="sxs-lookup"><span data-stu-id="ae344-184">The [UnreadCount](unreadcount.md) element is included in Tasks and Notes folders.</span></span> 
    
- <span data-ttu-id="ae344-185">Utilisez la valeur **PropertyTag** de 0x672D avec une propriété de type **Integer** pour identifier un dossier géré à l’aide de l’élément [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="ae344-185">Use the **PropertyTag** value of 0x672D with a property type of **Integer** to identify a managed folder by using the [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="ae344-186">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ae344-186">See also</span></span>



[<span data-ttu-id="ae344-187">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="ae344-187">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

