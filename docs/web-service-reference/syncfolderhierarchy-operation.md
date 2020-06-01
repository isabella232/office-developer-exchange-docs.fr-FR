---
title: Opération Opérationsyncfolderhierarchy
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchy
api_type:
- schema
ms.assetid: b31916b1-bc6c-4451-a475-b7c5417f752d
description: L’opération Opérationsyncfolderhierarchy synchronise les dossiers entre l’ordinateur qui exécute Microsoft Exchange Server 2010 et le client.
ms.openlocfilehash: 1c7ad2413064161ba54e8a7a30bfcd6f23f218bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456429"
---
# <a name="syncfolderhierarchy-operation"></a><span data-ttu-id="dff10-103">Opération Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="dff10-103">SyncFolderHierarchy operation</span></span>

<span data-ttu-id="dff10-104">L’opération Opérationsyncfolderhierarchy synchronise les dossiers entre l’ordinateur qui exécute Microsoft Exchange Server 2010 et le client.</span><span class="sxs-lookup"><span data-stu-id="dff10-104">The SyncFolderHierarchy operation synchronizes folders between the computer that is running Microsoft Exchange Server 2010 and the client.</span></span>
  
> [!NOTE]
> <span data-ttu-id="dff10-105">L’opération Opérationsyncfolderhierarchy ne renvoie pas de dossiers lorsque les propriétés [UnreadCount](unreadcount.md) ou [totalCount](totalcount.md) ont été modifiées.</span><span class="sxs-lookup"><span data-stu-id="dff10-105">The SyncFolderHierarchy operation does not return folders when the [UnreadCount](unreadcount.md) or [TotalCount](totalcount.md) properties have changed.</span></span> 
  
## <a name="syncfolderhierarchy-request-example"></a><span data-ttu-id="dff10-106">Exemple de requête Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="dff10-106">SyncFolderHierarchy request example</span></span>

### <a name="description"></a><span data-ttu-id="dff10-107">Description</span><span class="sxs-lookup"><span data-stu-id="dff10-107">Description</span></span>

<span data-ttu-id="dff10-108">L’exemple de requête Opérationsyncfolderhierarchy suivant montre comment synchroniser une hiérarchie de dossiers client avec le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="dff10-108">The following example of a SyncFolderHierarchy request shows how to synchronize a client folder hierarchy with the Exchange server.</span></span> <span data-ttu-id="dff10-109">Cet exemple montre une hiérarchie de dossiers qui a déjà été synchronisée au moins une fois.</span><span class="sxs-lookup"><span data-stu-id="dff10-109">This example shows a folder hierarchy that has already been synchronized at least one time.</span></span> <span data-ttu-id="dff10-110">L’élément [SyncState](syncstate-ex15websvcsotherref.md) n’est pas inclus dans la demande de la première tentative de synchronisation d’un client avec le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="dff10-110">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="dff10-111">La première demande renverra tous les dossiers de la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="dff10-111">The first request will return all the folders in the mailbox.</span></span> <span data-ttu-id="dff10-112">L’élément [SyncState](syncstate-ex15websvcsotherref.md) sera renvoyé dans le [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span><span class="sxs-lookup"><span data-stu-id="dff10-112">The [SyncState](syncstate-ex15websvcsotherref.md) element will be returned in the [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span></span> <span data-ttu-id="dff10-113">Cet élément est utilisé pour synchroniser l’état des demandes Opérationsyncfolderhierarchy suivantes.</span><span class="sxs-lookup"><span data-stu-id="dff10-113">This element is used to synchronize the state for subsequent SyncFolderHierarchy requests.</span></span>
  
### <a name="code"></a><span data-ttu-id="dff10-114">Code</span><span class="sxs-lookup"><span data-stu-id="dff10-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="dff10-115">Commentaires</span><span class="sxs-lookup"><span data-stu-id="dff10-115">Comments</span></span>

<span data-ttu-id="dff10-116">L’élément [SyncState](syncstate-ex15websvcsotherref.md) les données codées en base64 ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="dff10-116">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="dff10-117">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="dff10-117">Request elements</span></span>

<span data-ttu-id="dff10-118">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="dff10-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="dff10-119">Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="dff10-119">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md)
    
- [<span data-ttu-id="dff10-120">FolderShape</span><span class="sxs-lookup"><span data-stu-id="dff10-120">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="dff10-121">BaseShape</span><span class="sxs-lookup"><span data-stu-id="dff10-121">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="dff10-122">SyncState</span><span class="sxs-lookup"><span data-stu-id="dff10-122">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> <span data-ttu-id="dff10-123">Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="dff10-123">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-syncfolderhierarchy-response"></a><span data-ttu-id="dff10-124">Réponse Opérationsyncfolderhierarchy réussie</span><span class="sxs-lookup"><span data-stu-id="dff10-124">Successful SyncFolderHierarchy Response</span></span>

### <a name="description"></a><span data-ttu-id="dff10-125">Description</span><span class="sxs-lookup"><span data-stu-id="dff10-125">Description</span></span>

<span data-ttu-id="dff10-126">L’exemple suivant montre une réponse réussie à la demande Opérationsyncfolderhierarchy.</span><span class="sxs-lookup"><span data-stu-id="dff10-126">The following example shows a successful response to the SyncFolderHierarchy request.</span></span> <span data-ttu-id="dff10-127">Dans cet exemple, un nouveau dossier a été synchronisé.</span><span class="sxs-lookup"><span data-stu-id="dff10-127">In this example, a new folder has been synchronized.</span></span>
  
### <a name="code"></a><span data-ttu-id="dff10-128">Code</span><span class="sxs-lookup"><span data-stu-id="dff10-128">Code</span></span>

```XML
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
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SyncState>H4sIAAA==</m:SyncState>
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
          <m:Changes>
            <t:Create>
              <t:Folder>
                <t:FolderId Id="AQApAHR=" ChangeKey="AQAAABY" />
                <t:ParentFolderId Id="AQApA=" ChangeKey="AQAAAA==" />
                <t:FolderClass>IPF.Note</t:FolderClass>
                <t:DisplayName>NewFolder</t:DisplayName>
                <t:TotalCount>0</t:TotalCount>
                <t:ChildFolderCount>0</t:ChildFolderCount>
                <t:UnreadCount>0</t:UnreadCount>
              </t:Folder>
            </t:Create>
          </m:Changes>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="dff10-129">Commentaires</span><span class="sxs-lookup"><span data-stu-id="dff10-129">Comments</span></span>

<span data-ttu-id="dff10-130">L’élément [SyncState](syncstate-ex15websvcsotherref.md) données codées en base64 et les données de l’identificateur de dossier ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="dff10-130">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the folder identifier data have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="dff10-131">Éléments de réponse réussis</span><span class="sxs-lookup"><span data-stu-id="dff10-131">Successful response elements</span></span>

<span data-ttu-id="dff10-132">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="dff10-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="dff10-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="dff10-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="dff10-134">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="dff10-134">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="dff10-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dff10-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="dff10-136">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dff10-136">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="dff10-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dff10-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="dff10-138">SyncState</span><span class="sxs-lookup"><span data-stu-id="dff10-138">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="dff10-139">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="dff10-139">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
- [<span data-ttu-id="dff10-140">Changes (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="dff10-140">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
    
- [<span data-ttu-id="dff10-141">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="dff10-141">Create (FolderSync)</span></span>](create-foldersync.md)
    
- [<span data-ttu-id="dff10-142">Folder</span><span class="sxs-lookup"><span data-stu-id="dff10-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="dff10-143">FolderId</span><span class="sxs-lookup"><span data-stu-id="dff10-143">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="dff10-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="dff10-144">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="dff10-145">FolderClass</span><span class="sxs-lookup"><span data-stu-id="dff10-145">FolderClass</span></span>](folderclass.md)
    
- [<span data-ttu-id="dff10-146">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="dff10-146">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="dff10-147">TotalCount</span><span class="sxs-lookup"><span data-stu-id="dff10-147">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="dff10-148">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="dff10-148">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="dff10-149">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="dff10-149">UnreadCount</span></span>](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a><span data-ttu-id="dff10-150">Réponse d’erreur Opérationsyncfolderhierarchy</span><span class="sxs-lookup"><span data-stu-id="dff10-150">SyncFolderHierarchy error response</span></span>

### <a name="description"></a><span data-ttu-id="dff10-151">Description</span><span class="sxs-lookup"><span data-stu-id="dff10-151">Description</span></span>

<span data-ttu-id="dff10-152">L’exemple suivant montre une réponse d’erreur à une requête Opérationsyncfolderhierarchy.</span><span class="sxs-lookup"><span data-stu-id="dff10-152">The following example shows an error response to a SyncFolderHierarchy request.</span></span> <span data-ttu-id="dff10-153">Cette erreur a été causée par un SyncState non valide.</span><span class="sxs-lookup"><span data-stu-id="dff10-153">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="dff10-154">Code</span><span class="sxs-lookup"><span data-stu-id="dff10-154">Code</span></span>

```XML
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
    <SyncFolderHierarchyResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SyncFolderHierarchyResponseMessage ResponseClass="Error">
          <m:MessageText>Synchronization state data is corrupted or otherwise invalid.</m:MessageText>
          <m:ResponseCode>ErrorInvalidSyncStateData</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:SyncState />
          <m:IncludesLastFolderInRange>true</m:IncludesLastFolderInRange>
        </m:SyncFolderHierarchyResponseMessage>
      </m:ResponseMessages>
    </SyncFolderHierarchyResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="dff10-155">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="dff10-155">Error response elements</span></span>

<span data-ttu-id="dff10-156">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="dff10-156">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="dff10-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="dff10-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="dff10-158">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="dff10-158">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="dff10-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="dff10-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="dff10-160">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dff10-160">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="dff10-161">MessageText</span><span class="sxs-lookup"><span data-stu-id="dff10-161">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="dff10-162">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dff10-162">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="dff10-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="dff10-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="dff10-164">SyncState</span><span class="sxs-lookup"><span data-stu-id="dff10-164">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="dff10-165">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="dff10-165">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
## <a name="see-also"></a><span data-ttu-id="dff10-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dff10-166">See also</span></span>



- [<span data-ttu-id="dff10-167">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dff10-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

