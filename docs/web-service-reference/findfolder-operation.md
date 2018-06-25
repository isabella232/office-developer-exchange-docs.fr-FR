---
title: FindFolder Operation
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
description: L’opération FindFolder utilise les Services Web Exchange pour rechercher les sous-dossiers d’un dossier donné et retourne un ensemble de propriétés qui décrivent l’ensemble de sous-dossiers.
ms.openlocfilehash: 655455b46d4a3192b294bee9d85352d95ded49ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756386"
---
# <a name="findfolder-operation"></a><span data-ttu-id="589bb-103">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="589bb-103">FindFolder operation</span></span>

<span data-ttu-id="589bb-104">L’opération **FindFolder** utilise les Services Web Exchange pour rechercher les sous-dossiers d’un dossier donné et retourne un ensemble de propriétés qui décrivent l’ensemble de sous-dossiers.</span><span class="sxs-lookup"><span data-stu-id="589bb-104">The **FindFolder** operation uses Exchange Web Services to find subfolders of an identified folder and returns a set of properties that describe the set of subfolders.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="589bb-105">Remarques</span><span class="sxs-lookup"><span data-stu-id="589bb-105">Remarks</span></span>

<span data-ttu-id="589bb-106">FindFolder renvoie uniquement les 512 octets de n’importe quelle propriété lisible en continu.</span><span class="sxs-lookup"><span data-stu-id="589bb-106">FindFolder returns only the first 512 bytes of any streamable property.</span></span> <span data-ttu-id="589bb-107">Pour le format Unicode, elle renvoie les 255 premiers caractères à l’aide d’une chaîne Unicode terminée par null.</span><span class="sxs-lookup"><span data-stu-id="589bb-107">For Unicode, it returns the first 255 characters by using a null-terminated Unicode string.</span></span>
  
<span data-ttu-id="589bb-108">Impossible d’effectuer des requêtes approfondies sur les dossiers publics.</span><span class="sxs-lookup"><span data-stu-id="589bb-108">Deep traversal queries cannot be performed on public folders.</span></span>
  
<span data-ttu-id="589bb-109">Restrictions sont autorisées et doivent utiliser uniquement les propriétés du dossier, pas les propriétés d’élément.</span><span class="sxs-lookup"><span data-stu-id="589bb-109">Restrictions are permitted and should use only the folder properties, not the item properties.</span></span> <span data-ttu-id="589bb-110">Les fonctionnalités de tri n’est pas disponible pour les réponses **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="589bb-110">Sorting functionality is not available for **FindFolder** responses.</span></span> <span data-ttu-id="589bb-111">Requêtes groupées ne sont pas disponibles pour les requêtes **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="589bb-111">Grouped queries are not available for **FindFolder** queries.</span></span> 
  
 <span data-ttu-id="589bb-112">**Remarque** L’opération **FindFolder** est également utilisée pour rechercher les dossiers gérés.</span><span class="sxs-lookup"><span data-stu-id="589bb-112">**Note** The **FindFolder** operation is also used to find managed folders.</span></span> 
  
### <a name="soap-headers"></a><span data-ttu-id="589bb-113">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="589bb-113">SOAP Headers</span></span>

<span data-ttu-id="589bb-114">L’opération **FindFolder** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="589bb-114">The **FindFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="589bb-115">**Header**</span><span class="sxs-lookup"><span data-stu-id="589bb-115">**Header**</span></span>|<span data-ttu-id="589bb-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="589bb-116">**Element**</span></span>|<span data-ttu-id="589bb-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="589bb-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="589bb-118">Emprunt d’identité</span><span class="sxs-lookup"><span data-stu-id="589bb-118">Impersonation</span></span>  <br/> |[<span data-ttu-id="589bb-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="589bb-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="589bb-120">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="589bb-120">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="589bb-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="589bb-121">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="589bb-122">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="589bb-122">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="589bb-123">Identifie la culture RFC3066 à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="589bb-123">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="589bb-124">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="589bb-124">RequestVersion</span></span>  <br/> |[<span data-ttu-id="589bb-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="589bb-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="589bb-126">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="589bb-126">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="589bb-127">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="589bb-127">ServerVersion</span></span>  <br/> |[<span data-ttu-id="589bb-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="589bb-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="589bb-129">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="589bb-129">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="589bb-130">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="589bb-130">TimeZoneContext</span></span>  <br/> |[<span data-ttu-id="589bb-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="589bb-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="589bb-132">Identifie le fuseau horaire à utiliser pour toutes les réponses à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="589bb-132">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="findfolder-request-example"></a><span data-ttu-id="589bb-133">Exemple de requête FindFolder</span><span class="sxs-lookup"><span data-stu-id="589bb-133">FindFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="589bb-134">Description</span><span class="sxs-lookup"><span data-stu-id="589bb-134">Description</span></span>

<span data-ttu-id="589bb-135">L’exemple suivant d’une demande **FindFolder** indique comment former une requête pour rechercher tous les dossiers situés dans une boîte de réception.</span><span class="sxs-lookup"><span data-stu-id="589bb-135">The following example of a **FindFolder** request shows how to form a request to find all the folders located in an Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="589bb-136">Code</span><span class="sxs-lookup"><span data-stu-id="589bb-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindFolder Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="589bb-137">Commentaires</span><span class="sxs-lookup"><span data-stu-id="589bb-137">Comments</span></span>

<span data-ttu-id="589bb-138">La réponse à l’aide de la valeur par défaut pour le [BaseShape](baseshape.md), cette propriété renvoie le nom du dossier, l’ID de dossier, le nombre de sous-dossiers, le nombre de dossiers enfants qui que se trouve dans le dossier et le nombre d’éléments non lus.</span><span class="sxs-lookup"><span data-stu-id="589bb-138">Using the Default value for the [BaseShape](baseshape.md), the response returns the folder name, the folder ID, the number of subfolders, the number of child folders found in the folder, and the count of unread items.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="589bb-139">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="589bb-139">Request elements</span></span>

<span data-ttu-id="589bb-140">Cette demande **FindFolder** comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="589bb-140">This **FindFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="589bb-141">FindFolder</span><span class="sxs-lookup"><span data-stu-id="589bb-141">FindFolder</span></span>](findfolder.md)
    
- [<span data-ttu-id="589bb-142">FolderShape</span><span class="sxs-lookup"><span data-stu-id="589bb-142">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="589bb-143">BaseShape</span><span class="sxs-lookup"><span data-stu-id="589bb-143">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="589bb-144">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="589bb-144">ParentFolderIds</span></span>](parentfolderids.md)
    
- [<span data-ttu-id="589bb-145">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="589bb-145">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
 <span data-ttu-id="589bb-146">Pour les éléments de demande **FindFolder** supplémentaires, voir le schéma.</span><span class="sxs-lookup"><span data-stu-id="589bb-146">For additional **FindFolder** request elements, see the schema.</span></span> 
  
## <a name="findfolder-response-example"></a><span data-ttu-id="589bb-147">Exemple de réponse FindFolder</span><span class="sxs-lookup"><span data-stu-id="589bb-147">FindFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="589bb-148">Description</span><span class="sxs-lookup"><span data-stu-id="589bb-148">Description</span></span>

<span data-ttu-id="589bb-149">L’exemple de corps Simple Object Access Protocol (SOAP) suivant montre une réponse positive à la demande **FindFolder** .</span><span class="sxs-lookup"><span data-stu-id="589bb-149">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **FindFolder** request.</span></span> <span data-ttu-id="589bb-150">La réponse contient les éléments qui sont renvoyées lorsque la valeur par défaut pour la [BaseShape](baseshape.md) est utilisée.</span><span class="sxs-lookup"><span data-stu-id="589bb-150">The response contains the elements that are returned when the Default value for the [BaseShape](baseshape.md) is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="589bb-151">L’ID de dossier et la clé de modification ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="589bb-151">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="589bb-152">Code</span><span class="sxs-lookup"><span data-stu-id="589bb-152">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="response-elements"></a><span data-ttu-id="589bb-153">Éléments de réponse</span><span class="sxs-lookup"><span data-stu-id="589bb-153">Response elements</span></span>

<span data-ttu-id="589bb-154">Les propriétés qui sont retournées dans la réponse sont déterminées par le [BaseShape](baseshape.md) et [AdditionalProperties](additionalproperties.md) si elles sont utilisées.</span><span class="sxs-lookup"><span data-stu-id="589bb-154">The properties that are returned in the response are determined by the [BaseShape](baseshape.md) and the [AdditionalProperties](additionalproperties.md) if they are used.</span></span> <span data-ttu-id="589bb-155">Une réponse positive de **FindFolder** comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="589bb-155">A successful **FindFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="589bb-156">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="589bb-156">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="589bb-157">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="589bb-157">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="589bb-158">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="589bb-158">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="589bb-159">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="589bb-159">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
    
- [<span data-ttu-id="589bb-160">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="589bb-160">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="589bb-161">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="589bb-161">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md)
    
- [<span data-ttu-id="589bb-162">Dossiers</span><span class="sxs-lookup"><span data-stu-id="589bb-162">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="589bb-163">Folder</span><span class="sxs-lookup"><span data-stu-id="589bb-163">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="589bb-164">FolderId</span><span class="sxs-lookup"><span data-stu-id="589bb-164">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="589bb-165">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="589bb-165">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="589bb-166">TotalCount</span><span class="sxs-lookup"><span data-stu-id="589bb-166">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="589bb-167">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="589bb-167">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="589bb-168">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="589bb-168">UnreadCount</span></span>](unreadcount.md)
    
### <a name="comments"></a><span data-ttu-id="589bb-169">Commentaires</span><span class="sxs-lookup"><span data-stu-id="589bb-169">Comments</span></span>

 <span data-ttu-id="589bb-170">**FindFolder** réponses à une demande de la forme de réponse **AllProperties** ne renvoient pas [TotalCount](totalcount.md) et éléments [UnreadCount](unreadcount.md) pour les recherches de dossier public.</span><span class="sxs-lookup"><span data-stu-id="589bb-170">**FindFolder** responses to a request with the **AllProperties** response shape will not return the [TotalCount](totalcount.md) and [UnreadCount](unreadcount.md) elements for public folder searches.</span></span> 
  
## <a name="findfolder-error-response-example"></a><span data-ttu-id="589bb-171">Exemple de réponse d’erreur FindFolder</span><span class="sxs-lookup"><span data-stu-id="589bb-171">FindFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="589bb-172">Description</span><span class="sxs-lookup"><span data-stu-id="589bb-172">Description</span></span>

<span data-ttu-id="589bb-173">L’exemple de corps SOAP suivante montre une réponse d’erreur qui se produit lorsque vous recherchez un dossier identifié par un identificateur de dossier incorrect.</span><span class="sxs-lookup"><span data-stu-id="589bb-173">The following SOAP body example shows an error response that occurs when you search for a folder that is identified by a malformed folder identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="589bb-174">Code</span><span class="sxs-lookup"><span data-stu-id="589bb-174">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="652" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="589bb-175">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="589bb-175">Error response elements</span></span>

<span data-ttu-id="589bb-176">La réponse d’erreur **FindFolder** comprend les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="589bb-176">The **FindFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="589bb-177">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="589bb-177">FindFolderResponse</span></span>](findfolderresponse.md)
    
- [<span data-ttu-id="589bb-178">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="589bb-178">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="589bb-179">MessageText</span><span class="sxs-lookup"><span data-stu-id="589bb-179">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="589bb-180">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="589bb-180">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="589bb-181">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="589bb-181">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="additional-information"></a><span data-ttu-id="589bb-182">Informations supplémentaires</span><span class="sxs-lookup"><span data-stu-id="589bb-182">Additional Information</span></span>

- <span data-ttu-id="589bb-183">L’élément [DisplayName (string)](displayname-string.md) de dossier est toujours inclus dans la forme par défaut.</span><span class="sxs-lookup"><span data-stu-id="589bb-183">The folder [DisplayName (string)](displayname-string.md) element is always included in the default shape.</span></span> 
    
- <span data-ttu-id="589bb-184">L’élément [UnreadCount](unreadcount.md) est inclus dans les dossiers de tâches et de Notes.</span><span class="sxs-lookup"><span data-stu-id="589bb-184">The [UnreadCount](unreadcount.md) element is included in Tasks and Notes folders.</span></span> 
    
- <span data-ttu-id="589bb-185">Utilisez la valeur de **PropertyTag** de 0x672D avec un type de propriété de **nombre entier** pour identifier un dossier géré à l’aide de l’élément [ExtendedFieldURI](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="589bb-185">Use the **PropertyTag** value of 0x672D with a property type of **Integer** to identify a managed folder by using the [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="589bb-186">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="589bb-186">See also</span></span>



[<span data-ttu-id="589bb-187">Recherche de dossiers</span><span class="sxs-lookup"><span data-stu-id="589bb-187">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

