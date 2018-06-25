---
title: Opération GetSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolder
api_type:
- schema
ms.assetid: 75fee92a-a7f8-4a62-ad2b-17acbaada186
description: L’opération GetSharingFolder Obtient l’identificateur de dossier local d’un dossier partagé spécifié.
ms.openlocfilehash: 23adb10b22623fcbc1dd6b33bd674afafdaa8b19
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827670"
---
# <a name="getsharingfolder-operation"></a><span data-ttu-id="d2640-103">Opération GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="d2640-103">GetSharingFolder operation</span></span>

<span data-ttu-id="d2640-104">L’opération **GetSharingFolder** Obtient l’identificateur de dossier local d’un dossier partagé spécifié.</span><span class="sxs-lookup"><span data-stu-id="d2640-104">The **GetSharingFolder** operation gets the local folder identifier of a specified shared folder.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="d2640-105">En-têtes SOAP</span><span class="sxs-lookup"><span data-stu-id="d2640-105">SOAP Headers</span></span>

<span data-ttu-id="d2640-106">L’opération **GetSharingFolder** permettre utiliser les en-têtes SOAP qui sont répertoriés et décrits dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="d2640-106">The **GetSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="d2640-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="d2640-107">**Header**</span></span>|<span data-ttu-id="d2640-108">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d2640-108">**Element**</span></span>|<span data-ttu-id="d2640-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="d2640-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d2640-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="d2640-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="d2640-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d2640-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d2640-112">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="d2640-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="d2640-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="d2640-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="d2640-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d2640-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d2640-115">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="d2640-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getsharingfolder-request-example"></a><span data-ttu-id="d2640-116">Exemple de requête GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="d2640-116">GetSharingFolder request example</span></span>

### <a name="getting-the-local-folder-identifier-by-specifying-the-sharedfolderid-element-of-the-folder-being-shared"></a><span data-ttu-id="d2640-117">Obtention de l’identificateur de dossier Local en spécifiant l’élément SharedFolderId du dossier partagé</span><span class="sxs-lookup"><span data-stu-id="d2640-117">Getting the Local Folder Identifier by Specifying the SharedFolderId Element of the Folder Being Shared</span></span>

<span data-ttu-id="d2640-118">L’exemple de code suivant montre comment former une demande pour obtenir l’identificateur du dossier local qui correspond au dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="d2640-118">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="d2640-119">Le dossier partagé est identifié par l’adresse SMTP de la boîte aux lettres qui contient le dossier partagé et à l’élément [SharedFolderId](sharedfolderid.md) qui représente l’identificateur de ce dossier.</span><span class="sxs-lookup"><span data-stu-id="d2640-119">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [SharedFolderId](sharedfolderid.md) element that represents the identifier of that folder.</span></span> <span data-ttu-id="d2640-120">Dans cet exemple, le dossier partagé est la propriété par user1@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="d2640-120">In this example, the folder that is being shared is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d2640-121">Code</span><span class="sxs-lookup"><span data-stu-id="d2640-121">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:SharedFolderId>AAMkA=</m:SharedFolderId>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="getting-the-local-folder-identifier-by-specifying-the-datatype-element-of-the-folder-being-shared"></a><span data-ttu-id="d2640-122">Obtention de l’identificateur de dossier Local en spécifiant l’élément de type de données du dossier partagé</span><span class="sxs-lookup"><span data-stu-id="d2640-122">Getting the Local Folder Identifier by Specifying the DataType Element of the Folder Being Shared</span></span>

<span data-ttu-id="d2640-123">L’exemple de code suivant montre comment former une demande pour obtenir l’identificateur du dossier local qui correspond au dossier partagé.</span><span class="sxs-lookup"><span data-stu-id="d2640-123">The following code example shows how to form a request to get the identifier of the local folder that corresponds to the folder that is being shared.</span></span> <span data-ttu-id="d2640-124">Le dossier partagé est identifié par l’adresse SMTP de la boîte aux lettres qui contient le dossier partagé et à l’élément de [type de données](datatype.md) qui représente le type de données dans ce dossier.</span><span class="sxs-lookup"><span data-stu-id="d2640-124">The folder that is being shared is identified by the SMTP address of the mailbox that contains the folder that is being shared and by the [DataType](datatype.md) element that represents the type of data in that folder.</span></span> <span data-ttu-id="d2640-125">Dans cet exemple, le dossier partagé est le dossier Contacts appartenant à user1@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="d2640-125">In this example, the folder that is being shared is the Contacts folder that is owned by user1@contoso.com.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d2640-126">Code</span><span class="sxs-lookup"><span data-stu-id="d2640-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetSharingFolder>
      <m:SmtpAddress>user1@contoso.com</m:SmtpAddress>
      <m:DataType>Contacts</m:DataType>
    </m:GetSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d2640-127">Commentaires</span><span class="sxs-lookup"><span data-stu-id="d2640-127">Comments</span></span>

<span data-ttu-id="d2640-128">Pour plus d’informations sur les valeurs possibles de l’élément de **type de données** , voir [le type de données](datatype.md).</span><span class="sxs-lookup"><span data-stu-id="d2640-128">For information about the possible values of the **DataType** element, see [DataType](datatype.md).</span></span>
  
## <a name="successful-getsharingfolder-response"></a><span data-ttu-id="d2640-129">Réponse GetSharingFolder réussie</span><span class="sxs-lookup"><span data-stu-id="d2640-129">Successful GetSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="d2640-130">Description</span><span class="sxs-lookup"><span data-stu-id="d2640-130">Description</span></span>

<span data-ttu-id="d2640-131">L’exemple suivant montre une réponse positive à une demande de **GetSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="d2640-131">The following example shows a successful response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="d2640-132">L’attribut **Id** de l’élément [SharingFolderId](sharingfolderid.md) représente l’identificateur du dossier local dans la relation de partage.</span><span class="sxs-lookup"><span data-stu-id="d2640-132">The **Id** attribute of the [SharingFolderId](sharingfolderid.md) element represents the identifier of the local folder in the sharing relationship.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d2640-133">Code</span><span class="sxs-lookup"><span data-stu-id="d2640-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="getsharingfolder-error-response"></a><span data-ttu-id="d2640-134">Réponse d’erreur GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="d2640-134">GetSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="d2640-135">Description</span><span class="sxs-lookup"><span data-stu-id="d2640-135">Description</span></span>

<span data-ttu-id="d2640-136">L’exemple suivant montre une réponse d’erreur à une demande de **GetSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="d2640-136">The following example shows an error response to a **GetSharingFolder** request.</span></span> <span data-ttu-id="d2640-137">Cet exemple, l’erreur s’est produite, car la demande a spécifié le [SharingFolderId](sharingfolderid.md) et le [type de données](datatype.md) des éléments.</span><span class="sxs-lookup"><span data-stu-id="d2640-137">In this example, the error occurred because the request specified both the [SharingFolderId](sharingfolderid.md) and [DataType](datatype.md) elements.</span></span> <span data-ttu-id="d2640-138">Notez que seul l’un ou l’autre de ces deux éléments peut être spécifiée, mais pas les deux.</span><span class="sxs-lookup"><span data-stu-id="d2640-138">Note that only one or the other of those two elements can be specified, but not both.</span></span> 
  
### <a name="code"></a><span data-ttu-id="d2640-139">Code</span><span class="sxs-lookup"><span data-stu-id="d2640-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetSharingFolderResponseMessage ResponseClass="Error" 
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Either DataType or SharedFolderId must be specified, but not both.</m:MessageText>
      <m:ResponseCode>ErrorInvalidGetSharingFolderRequest</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
    </GetSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="d2640-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d2640-140">See also</span></span>



[<span data-ttu-id="d2640-141">GetSharingFolder</span><span class="sxs-lookup"><span data-stu-id="d2640-141">GetSharingFolder</span></span>](getsharingfolder.md)
  
[<span data-ttu-id="d2640-142">GetSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="d2640-142">GetSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderType.aspx)
  
[<span data-ttu-id="d2640-143">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d2640-143">GetSharingFolderResponseMessage</span></span>](getsharingfolderresponsemessage.md)
  
[<span data-ttu-id="d2640-144">GetSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="d2640-144">GetSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.GetSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="d2640-145">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d2640-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="d2640-146">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d2640-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

