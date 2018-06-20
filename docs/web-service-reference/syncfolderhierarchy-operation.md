---
title: Opération SyncFolderHierarchy
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
description: L’opération SyncFolderHierarchy synchronise les dossiers entre l’ordinateur qui exécute Microsoft Exchange Server 2010 et le client.
ms.openlocfilehash: 33c886d5eec64a9ff2ccc667eedfc2d4cc8dcfd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838657"
---
# <a name="syncfolderhierarchy-operation"></a><span data-ttu-id="c3324-103">Opération SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="c3324-103">SyncFolderHierarchy operation</span></span>

<span data-ttu-id="c3324-104">L’opération SyncFolderHierarchy synchronise les dossiers entre l’ordinateur qui exécute Microsoft Exchange Server 2010 et le client.</span><span class="sxs-lookup"><span data-stu-id="c3324-104">The SyncFolderHierarchy operation synchronizes folders between the computer that is running Microsoft Exchange Server 2010 and the client.</span></span>
  
> [!NOTE]
> <span data-ttu-id="c3324-105">L’opération SyncFolderHierarchy ne renvoie pas les dossiers lorsque les propriétés [UnreadCount](unreadcount.md) ou [TotalCount](totalcount.md) ont changé.</span><span class="sxs-lookup"><span data-stu-id="c3324-105">The SyncFolderHierarchy operation does not return folders when the [UnreadCount](unreadcount.md) or [TotalCount](totalcount.md) properties have changed.</span></span> 
  
## <a name="syncfolderhierarchy-request-example"></a><span data-ttu-id="c3324-106">Exemple de requête SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="c3324-106">SyncFolderHierarchy request example</span></span>

### <a name="description"></a><span data-ttu-id="c3324-107">Description</span><span class="sxs-lookup"><span data-stu-id="c3324-107">Description</span></span>

<span data-ttu-id="c3324-108">L’exemple suivant d’une demande SyncFolderHierarchy montre comment synchroniser un client de hiérarchie de dossiers avec le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3324-108">The following example of a SyncFolderHierarchy request shows how to synchronize a client folder hierarchy with the Exchange server.</span></span> <span data-ttu-id="c3324-109">Cet exemple montre une hiérarchie de dossiers qui a déjà été synchronisée au moins une fois.</span><span class="sxs-lookup"><span data-stu-id="c3324-109">This example shows a folder hierarchy that has already been synchronized at least one time.</span></span> <span data-ttu-id="c3324-110">L’élément [SyncState](syncstate-ex15websvcsotherref.md) n’est pas inclus dans la demande de la première tentative de synchroniser un client avec le serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="c3324-110">The [SyncState](syncstate-ex15websvcsotherref.md) element is not included in the request for the first attempt to synchronize a client with the Exchange server.</span></span> <span data-ttu-id="c3324-111">La première requête retournera tous les dossiers dans la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="c3324-111">The first request will return all the folders in the mailbox.</span></span> <span data-ttu-id="c3324-112">L’élément [SyncState](syncstate-ex15websvcsotherref.md) est renvoyé dans la [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span><span class="sxs-lookup"><span data-stu-id="c3324-112">The [SyncState](syncstate-ex15websvcsotherref.md) element will be returned in the [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md).</span></span> <span data-ttu-id="c3324-113">Cet élément est utilisé pour synchroniser l’état pour les demandes SyncFolderHierarchy suivantes.</span><span class="sxs-lookup"><span data-stu-id="c3324-113">This element is used to synchronize the state for subsequent SyncFolderHierarchy requests.</span></span>
  
### <a name="code"></a><span data-ttu-id="c3324-114">Code</span><span class="sxs-lookup"><span data-stu-id="c3324-114">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SyncFolderHierarchy  xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </FolderShape>
      <SyncState>H4sIA=</SyncState>
    </SyncFolderHierarchy>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="c3324-115">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c3324-115">Comments</span></span>

<span data-ttu-id="c3324-116">Les données d’élément codée en base64 [SyncState](syncstate-ex15websvcsotherref.md) a été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c3324-116">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data has been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="c3324-117">Éléments de la demande</span><span class="sxs-lookup"><span data-stu-id="c3324-117">Request elements</span></span>

<span data-ttu-id="c3324-118">Les éléments suivants sont utilisés dans la demande :</span><span class="sxs-lookup"><span data-stu-id="c3324-118">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c3324-119">SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="c3324-119">SyncFolderHierarchy</span></span>](syncfolderhierarchy.md)
    
- [<span data-ttu-id="c3324-120">FolderShape</span><span class="sxs-lookup"><span data-stu-id="c3324-120">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="c3324-121">BaseShape</span><span class="sxs-lookup"><span data-stu-id="c3324-121">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="c3324-122">SyncState</span><span class="sxs-lookup"><span data-stu-id="c3324-122">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
> [!NOTE]
> <span data-ttu-id="c3324-123">Le schéma qui décrit ces éléments se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute MicrosoftExchange Server 2007 ayant le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="c3324-123">The schema that describes these elements is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="successful-syncfolderhierarchy-response"></a><span data-ttu-id="c3324-124">Réponse SyncFolderHierarchy réussie</span><span class="sxs-lookup"><span data-stu-id="c3324-124">Successful SyncFolderHierarchy Response</span></span>

### <a name="description"></a><span data-ttu-id="c3324-125">Description</span><span class="sxs-lookup"><span data-stu-id="c3324-125">Description</span></span>

<span data-ttu-id="c3324-126">L’exemple suivant montre une réponse positive à la demande SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="c3324-126">The following example shows a successful response to the SyncFolderHierarchy request.</span></span> <span data-ttu-id="c3324-127">Dans cet exemple, un nouveau dossier a été synchronisé.</span><span class="sxs-lookup"><span data-stu-id="c3324-127">In this example, a new folder has been synchronized.</span></span>
  
### <a name="code"></a><span data-ttu-id="c3324-128">Code</span><span class="sxs-lookup"><span data-stu-id="c3324-128">Code</span></span>

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
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="c3324-129">Commentaires</span><span class="sxs-lookup"><span data-stu-id="c3324-129">Comments</span></span>

<span data-ttu-id="c3324-130">Les données d’élément codée en base64 [SyncState](syncstate-ex15websvcsotherref.md) et les données d’identificateur de dossier ont été réduites afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c3324-130">The [SyncState](syncstate-ex15websvcsotherref.md) element base64-encoded data and the folder identifier data have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="c3324-131">Éléments de réponse réussie</span><span class="sxs-lookup"><span data-stu-id="c3324-131">Successful response elements</span></span>

<span data-ttu-id="c3324-132">Les éléments suivants sont utilisés dans la réponse :</span><span class="sxs-lookup"><span data-stu-id="c3324-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c3324-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c3324-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c3324-134">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="c3324-134">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="c3324-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c3324-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c3324-136">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c3324-136">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="c3324-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c3324-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c3324-138">SyncState</span><span class="sxs-lookup"><span data-stu-id="c3324-138">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c3324-139">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="c3324-139">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
- [<span data-ttu-id="c3324-140">Modifications (hiérarchie)</span><span class="sxs-lookup"><span data-stu-id="c3324-140">Changes (Hierarchy)</span></span>](changes-hierarchy.md)
    
- [<span data-ttu-id="c3324-141">Créer (FolderSync)</span><span class="sxs-lookup"><span data-stu-id="c3324-141">Create (FolderSync)</span></span>](create-foldersync.md)
    
- [<span data-ttu-id="c3324-142">Folder</span><span class="sxs-lookup"><span data-stu-id="c3324-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="c3324-143">FolderId</span><span class="sxs-lookup"><span data-stu-id="c3324-143">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="c3324-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="c3324-144">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="c3324-145">Classe FolderClass</span><span class="sxs-lookup"><span data-stu-id="c3324-145">FolderClass</span></span>](folderclass.md)
    
- [<span data-ttu-id="c3324-146">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="c3324-146">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="c3324-147">TotalCount</span><span class="sxs-lookup"><span data-stu-id="c3324-147">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="c3324-148">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="c3324-148">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="c3324-149">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="c3324-149">UnreadCount</span></span>](unreadcount.md)
    
## <a name="syncfolderhierarchy-error-response"></a><span data-ttu-id="c3324-150">Réponse d’erreur SyncFolderHierarchy</span><span class="sxs-lookup"><span data-stu-id="c3324-150">SyncFolderHierarchy error response</span></span>

### <a name="description"></a><span data-ttu-id="c3324-151">Description</span><span class="sxs-lookup"><span data-stu-id="c3324-151">Description</span></span>

<span data-ttu-id="c3324-152">L’exemple suivant montre une réponse d’erreur à une demande SyncFolderHierarchy.</span><span class="sxs-lookup"><span data-stu-id="c3324-152">The following example shows an error response to a SyncFolderHierarchy request.</span></span> <span data-ttu-id="c3324-153">Cette erreur a été provoquée par une SyncState non valide.</span><span class="sxs-lookup"><span data-stu-id="c3324-153">This error was caused by an invalid SyncState.</span></span>
  
### <a name="code"></a><span data-ttu-id="c3324-154">Code</span><span class="sxs-lookup"><span data-stu-id="c3324-154">Code</span></span>

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
    <SyncFolderHierarchyResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="c3324-155">Éléments de réponse d’erreur</span><span class="sxs-lookup"><span data-stu-id="c3324-155">Error response elements</span></span>

<span data-ttu-id="c3324-156">Les éléments suivants sont utilisés dans la réponse d'erreur :</span><span class="sxs-lookup"><span data-stu-id="c3324-156">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="c3324-157">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c3324-157">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c3324-158">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="c3324-158">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md)
    
- [<span data-ttu-id="c3324-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c3324-159">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c3324-160">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c3324-160">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
    
- [<span data-ttu-id="c3324-161">MessageText</span><span class="sxs-lookup"><span data-stu-id="c3324-161">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c3324-162">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c3324-162">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c3324-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c3324-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="c3324-164">SyncState</span><span class="sxs-lookup"><span data-stu-id="c3324-164">SyncState</span></span>](syncstate-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c3324-165">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="c3324-165">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md)
    
## <a name="see-also"></a><span data-ttu-id="c3324-166">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c3324-166">See also</span></span>



- [<span data-ttu-id="c3324-167">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c3324-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

