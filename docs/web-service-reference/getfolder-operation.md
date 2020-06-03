---
title: Opération GetFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetFolder
api_type:
- schema
ms.assetid: 355bcf93-dc71-4493-b177-622afac5fdb9
description: L’opération GetFolder obtient des dossiers à partir de la Banque d’Exchange.
localization_priority: Priority
ms.openlocfilehash: 9d511f309b9210fd9b5a49ff6c60bc7982992973
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459180"
---
# <a name="getfolder-operation"></a><span data-ttu-id="c7058-103">Opération GetFolder</span><span class="sxs-lookup"><span data-stu-id="c7058-103">GetFolder operation</span></span>

<span data-ttu-id="c7058-104">L’opération **GetFolder** obtient des dossiers à partir de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7058-104">The **GetFolder** operation gets folders from the Exchange store.</span></span> 
  
## <a name="getfolder-request-example"></a><span data-ttu-id="c7058-105">Exemple de requête GetFolder</span><span class="sxs-lookup"><span data-stu-id="c7058-105">GetFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="c7058-106">Description</span><span class="sxs-lookup"><span data-stu-id="c7058-106">Description</span></span>

<span data-ttu-id="c7058-107">L’exemple de requête **GetFolder** suivant montre comment obtenir un identificateur de dossier, le nom d’affichage, le nombre d’éléments contenus dans ce dossier, le nombre de dossiers enfants et le nombre d’éléments non lus dans le dossier.</span><span class="sxs-lookup"><span data-stu-id="c7058-107">The following example of a **GetFolder** request shows how to obtain a folder identifier, display name, the count of items in that folder, the count of child folders, and the number of unread items in the folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c7058-108">Code</span><span class="sxs-lookup"><span data-stu-id="c7058-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
   xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetFolder xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <FolderShape>
        <t:BaseShape>Default</t:BaseShape>
      </FolderShape>
      <FolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </FolderIds>
    </GetFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="c7058-109">Demander des éléments</span><span class="sxs-lookup"><span data-stu-id="c7058-109">Request elements</span></span>

<span data-ttu-id="c7058-110">Cette demande **GetFolder** inclut les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="c7058-110">This **GetFolder** request includes the following elements:</span></span> 
  
- [<span data-ttu-id="c7058-111">GetFolder</span><span class="sxs-lookup"><span data-stu-id="c7058-111">GetFolder</span></span>](getfolder.md)
    
- [<span data-ttu-id="c7058-112">FolderShape</span><span class="sxs-lookup"><span data-stu-id="c7058-112">FolderShape</span></span>](foldershape.md)
    
- [<span data-ttu-id="c7058-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="c7058-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="c7058-114">FolderIds</span><span class="sxs-lookup"><span data-stu-id="c7058-114">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="c7058-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c7058-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="c7058-116">Consultez le schéma pour les éléments supplémentaires que vous pouvez utiliser pour créer une demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="c7058-116">See the schema for additional elements that you can use to form a **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c7058-117">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c7058-117">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span> 
  
## <a name="getfolder-response-example"></a><span data-ttu-id="c7058-118">Exemple de réponse GetFolder</span><span class="sxs-lookup"><span data-stu-id="c7058-118">GetFolder response example</span></span>

### <a name="description"></a><span data-ttu-id="c7058-119">Description</span><span class="sxs-lookup"><span data-stu-id="c7058-119">Description</span></span>

<span data-ttu-id="c7058-120">L’exemple de corps SOAP (Simple Object Access Protocol) suivant montre une réponse réussie à la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="c7058-120">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetFolder** request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c7058-121">L’ID de dossier et la clé de modification ont été raccourcies afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="c7058-121">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c7058-122">Code</span><span class="sxs-lookup"><span data-stu-id="c7058-122">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="AQApA=" ChangeKey="AQAAAB" />
              <t:DisplayName>Inbox</t:DisplayName>
              <t:TotalCount>2</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:UnreadCount>2</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </GetFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="c7058-123">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="c7058-123">Response elements</span></span>

<span data-ttu-id="c7058-124">Cette réponse **GetFolder** inclut les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="c7058-124">This **GetFolder** response includes the following elements:</span></span> 
  
- [<span data-ttu-id="c7058-125">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="c7058-125">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="c7058-126">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c7058-126">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c7058-127">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c7058-127">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="c7058-128">Dossiers</span><span class="sxs-lookup"><span data-stu-id="c7058-128">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="c7058-129">Folder</span><span class="sxs-lookup"><span data-stu-id="c7058-129">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="c7058-130">FolderId</span><span class="sxs-lookup"><span data-stu-id="c7058-130">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="c7058-131">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="c7058-131">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="c7058-132">TotalCount</span><span class="sxs-lookup"><span data-stu-id="c7058-132">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="c7058-133">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="c7058-133">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="c7058-134">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="c7058-134">UnreadCount</span></span>](unreadcount.md)
    
## <a name="getfolder-error-response-example"></a><span data-ttu-id="c7058-135">Exemple de réponse d’erreur GetFolder</span><span class="sxs-lookup"><span data-stu-id="c7058-135">GetFolder Error response example</span></span>

### <a name="description"></a><span data-ttu-id="c7058-136">Description</span><span class="sxs-lookup"><span data-stu-id="c7058-136">Description</span></span>

<span data-ttu-id="c7058-137">L’exemple de corps SOAP suivant montre une réponse d’erreur provoquée par un [FolderId](folderid.md) incorrect dans la demande.</span><span class="sxs-lookup"><span data-stu-id="c7058-137">The following SOAP body example shows an error response that is caused by an incorrect [FolderId](folderid.md) in the request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c7058-138">Code</span><span class="sxs-lookup"><span data-stu-id="c7058-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Folders />
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </GetFolderResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="c7058-139">Éléments Response</span><span class="sxs-lookup"><span data-stu-id="c7058-139">Response elements</span></span>

<span data-ttu-id="c7058-140">Cette réponse d’erreur **GetFolder** inclut les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="c7058-140">This **GetFolder** error response includes the following elements:</span></span> 
  
- [<span data-ttu-id="c7058-141">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="c7058-141">GetFolderResponse</span></span>](getfolderresponse.md)
    
- [<span data-ttu-id="c7058-142">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c7058-142">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c7058-143">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c7058-143">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
    
- [<span data-ttu-id="c7058-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="c7058-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c7058-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c7058-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c7058-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c7058-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="c7058-147">Dossiers</span><span class="sxs-lookup"><span data-stu-id="c7058-147">Folders</span></span>](folders-ex15websvcsotherref.md)
    
## <a name="version-differences"></a><span data-ttu-id="c7058-148">Différences entre les versions</span><span class="sxs-lookup"><span data-stu-id="c7058-148">Version differences</span></span>

<span data-ttu-id="c7058-149">Pour les applications qui ciblent Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange à partir d’Exchange 2013, les autorisations de dossiers ne sont pas renvoyées lorsque l’élément [BaseShape](baseshape.md) a une valeur de **AllProperties** dans la demande d’opération [GetFolder](getfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="c7058-149">For applications that target Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013, folder permissions are not returned when the [BaseShape](baseshape.md) element has a value of **AllProperties** in the [GetFolder](getfolder-operation.md) operation request.</span></span> <span data-ttu-id="c7058-150">Pour récupérer les autorisations de dossier, ajoutez l’élément [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) à l’élément [AdditionalProperties](additionalproperties.md) dans la demande **GetFolder** .</span><span class="sxs-lookup"><span data-stu-id="c7058-150">To retrieve folder permissions, add the [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) element to the [AdditionalProperties](additionalproperties.md) element in the **GetFolder** request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c7058-151">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c7058-151">See also</span></span>



- [<span data-ttu-id="c7058-152">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c7058-152">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

