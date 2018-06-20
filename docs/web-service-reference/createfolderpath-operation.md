---
title: Opération CreateFolderPath
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5a10aa5e-3f25-4ec3-a0b9-284c30918a1f
description: Opération de recherche plus d’informations sur la CreateFolderPath EWS.
ms.openlocfilehash: 22561e5086c144e25d7e04b68ec6674b87c4718d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755703"
---
# <a name="createfolderpath-operation"></a><span data-ttu-id="92d2f-103">Opération CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="92d2f-103">CreateFolderPath operation</span></span>

<span data-ttu-id="92d2f-104">Trouvez des informations sur l’opération EWS **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="92d2f-104">Find information about the **CreateFolderPath** EWS operation.</span></span> 
  
<span data-ttu-id="92d2f-105">L’opération **CreateFolderPath** crée une hiérarchie de dossiers.</span><span class="sxs-lookup"><span data-stu-id="92d2f-105">The **CreateFolderPath** operation creates a folder hierarchy.</span></span> 
  
<span data-ttu-id="92d2f-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="92d2f-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-createfolderpath-operation"></a><span data-ttu-id="92d2f-107">Utilisation de l’opération CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="92d2f-107">Using the CreateFolderPath operation</span></span>

<span data-ttu-id="92d2f-108">La requête d’opération **CreateFolderPath** prend un tableau de dossiers et un identificateur de dossier parent et crée une hiérarchie de dossiers selon l’ordre des dossiers dans le tableau.</span><span class="sxs-lookup"><span data-stu-id="92d2f-108">The **CreateFolderPath** operation request takes an array of folders and a parent folder identifier and creates a folder hierarchy based on the order of the folders in the array.</span></span> 
  
### <a name="createfolderpath-operation-soap-headers"></a><span data-ttu-id="92d2f-109">En-têtes SOAP CreateFolderPath opération</span><span class="sxs-lookup"><span data-stu-id="92d2f-109">CreateFolderPath operation SOAP headers</span></span>

<span data-ttu-id="92d2f-110">L’opération **CreateFolderPath** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="92d2f-110">The **CreateFolderPath** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="92d2f-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="92d2f-111">**Header name**</span></span>|<span data-ttu-id="92d2f-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="92d2f-112">**Element**</span></span>|<span data-ttu-id="92d2f-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="92d2f-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="92d2f-114">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="92d2f-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="92d2f-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="92d2f-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="92d2f-116">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="92d2f-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="92d2f-117">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="92d2f-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="92d2f-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="92d2f-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="92d2f-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="92d2f-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="92d2f-120">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="92d2f-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="92d2f-121">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="92d2f-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="92d2f-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="92d2f-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="92d2f-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="92d2f-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="92d2f-124">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="92d2f-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="92d2f-125">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="92d2f-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="92d2f-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="92d2f-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="92d2f-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="92d2f-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="92d2f-128">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="92d2f-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="92d2f-129">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="92d2f-129">This header is applicable to a response.</span></span>  <br/> |
|<span data-ttu-id="92d2f-130">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="92d2f-130">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="92d2f-131">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="92d2f-131">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="92d2f-132">Identifie l’étendue de fuseau horaire pour les propriétés de **DateTime** .</span><span class="sxs-lookup"><span data-stu-id="92d2f-132">Identifies the time zone scope for **DateTime** properties.</span></span> <span data-ttu-id="92d2f-133">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="92d2f-133">This header is applicable to a request.</span></span>  <br/> |
   
## <a name="createfolderpath-operation-request-example-create-a-folder-hierarchy"></a><span data-ttu-id="92d2f-134">Exemple de requête d’opération CreateFolderPath : créer une hiérarchie de dossiers</span><span class="sxs-lookup"><span data-stu-id="92d2f-134">CreateFolderPath operation request example: Create a folder hierarchy</span></span>

<span data-ttu-id="92d2f-135">Une demande d’opération **CreateFolderPath** l’exemple suivant montre comment créer une hiérarchie de dossiers est trois dossiers dans le dossier boîte de réception par défaut.</span><span class="sxs-lookup"><span data-stu-id="92d2f-135">The following example of a **CreateFolderPath** operation request shows how to create a folder hierarchy that is three folders deep in the default Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="92d2f-136">Tous les identificateurs d’article et modifier des clés dans cet article ont été réduits afin de préserver la lisibilité.</span><span class="sxs-lookup"><span data-stu-id="92d2f-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:CreateFolderPath>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ParentFolderId>
         <m:RelativeFolderPath>
            <t:Folder>
               <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MySecondLevelFolder</t:DisplayName>
            </t:Folder>
            <t:Folder>
               <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
            </t:Folder>
         </m:RelativeFolderPath>
      </m:CreateFolderPath>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="92d2f-137">La demande SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="92d2f-137">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="92d2f-138">CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="92d2f-138">CreateFolderPath</span></span>](createfolderpath.md)
    
- [<span data-ttu-id="92d2f-139">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="92d2f-139">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="92d2f-140">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="92d2f-140">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="92d2f-141">RelativeFolderPath</span><span class="sxs-lookup"><span data-stu-id="92d2f-141">RelativeFolderPath</span></span>](relativefolderpath.md)
    
- [<span data-ttu-id="92d2f-142">Folder</span><span class="sxs-lookup"><span data-stu-id="92d2f-142">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="92d2f-143">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="92d2f-143">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-createfolderpath-operation-response"></a><span data-ttu-id="92d2f-144">Réponse d’opération CreateFolderPath réussie</span><span class="sxs-lookup"><span data-stu-id="92d2f-144">Successful CreateFolderPath operation response</span></span>

<span data-ttu-id="92d2f-145">L’exemple suivant montre une réponse positive à une demande d’opération **CreateFolderPath** pour créer un dossier dossiers hiérarchie trois profondeur dans le dossier boîte de réception par défaut.</span><span class="sxs-lookup"><span data-stu-id="92d2f-145">The following example shows a successful response to a **CreateFolderPath** operation request to create a folder hierarchy three folders deep in the default Inbox folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExYisXAAA=" ChangeKey="AQAAABYAABq6Wxb"/>
                     <t:DisplayName>MyFirstLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTExm4QrAABqxisYAAA=" ChangeKey="AQAAABYAAAm4QrAABq6Wxg"/>
                     <t:DisplayName>MySecondLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Folders>
                  <t:Folder>
                     <t:FolderId Id="AAMkADEzOTAABqxisZAAA=" ChangeKey="AQAAABYAA6Wxl"/>
                     <t:DisplayName>MyThirdLevelFolder</t:DisplayName>
                     <t:TotalCount>0</t:TotalCount>
                     <t:ChildFolderCount>0</t:ChildFolderCount>
                     <t:UnreadCount>0</t:UnreadCount>
                  </t:Folder>
               </m:Folders>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="92d2f-146">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="92d2f-146">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="92d2f-147">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="92d2f-147">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="92d2f-148">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="92d2f-148">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="92d2f-149">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="92d2f-149">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="92d2f-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="92d2f-150">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="92d2f-151">Dossiers</span><span class="sxs-lookup"><span data-stu-id="92d2f-151">Folders</span></span>](folders-ex15websvcsotherref.md)
    
- [<span data-ttu-id="92d2f-152">Folder</span><span class="sxs-lookup"><span data-stu-id="92d2f-152">Folder</span></span>](folder.md)
    
- [<span data-ttu-id="92d2f-153">FolderId</span><span class="sxs-lookup"><span data-stu-id="92d2f-153">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="92d2f-154">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="92d2f-154">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="92d2f-155">TotalCount</span><span class="sxs-lookup"><span data-stu-id="92d2f-155">TotalCount</span></span>](totalcount.md)
    
- [<span data-ttu-id="92d2f-156">ChildFolderCount</span><span class="sxs-lookup"><span data-stu-id="92d2f-156">ChildFolderCount</span></span>](childfoldercount.md)
    
- [<span data-ttu-id="92d2f-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="92d2f-157">UnreadCount</span></span>](unreadcount.md)
    
## <a name="createfolderpath-operation-error-response"></a><span data-ttu-id="92d2f-158">Réponse d’erreur d’opération CreateFolderPath</span><span class="sxs-lookup"><span data-stu-id="92d2f-158">CreateFolderPath operation error response</span></span>

<span data-ttu-id="92d2f-159">L’exemple suivant montre une réponse d’erreur à une demande d’opération **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="92d2f-159">The following example shows an error response to a **CreateFolderPath** operation request.</span></span> <span data-ttu-id="92d2f-160">Il s’agit d’une réponse à une demande de créer deux dossiers, le premier d'entre eux n’est pas une propriété de nom d’affichage définie.</span><span class="sxs-lookup"><span data-stu-id="92d2f-160">This is a response to a request to create two folders, the first of which does not have a display name property set.</span></span> <span data-ttu-id="92d2f-161">Le premier dossier de la hiérarchie ne peut pas être créé sans une propriété de nom d’affichage et le dossier deuxième ne peut pas être créé, car le dossier parent dans la hiérarchie n’a pas été créé.</span><span class="sxs-lookup"><span data-stu-id="92d2f-161">The first folder in the hierarchy cannot be created without a display name property, and the second folder cannot be created because the parent folder in the hierarchy was not created.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:CreateFolderPathResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The folder save operation failed due to invalid property values.</m:MessageText>
               <m:ResponseCode>ErrorFolderSavePropertyError</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:MessageXml>
                  <t:FieldURI FieldURI="folder:DisplayName"/>
               </m:MessageXml>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
            <m:CreateFolderPathResponseMessage ResponseClass="Error">
               <m:MessageText>The specified parent folder could not be found.</m:MessageText>
               <m:ResponseCode>ErrorParentFolderNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Folders/>
            </m:CreateFolderPathResponseMessage>
         </m:ResponseMessages>
      </m:CreateFolderPathResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="92d2f-162">La réponse d’erreur corps SOAP contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="92d2f-162">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="92d2f-163">CreateFolderPathResponse</span><span class="sxs-lookup"><span data-stu-id="92d2f-163">CreateFolderPathResponse</span></span>](createfolderpathresponse.md)
    
- [<span data-ttu-id="92d2f-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="92d2f-164">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="92d2f-165">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="92d2f-165">CreateFolderPathResponseMessage</span></span>](createfolderpathresponsemessage.md)
    
- [<span data-ttu-id="92d2f-166">MessageText</span><span class="sxs-lookup"><span data-stu-id="92d2f-166">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="92d2f-167">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="92d2f-167">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="92d2f-168">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="92d2f-168">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="92d2f-169">MessageXml</span><span class="sxs-lookup"><span data-stu-id="92d2f-169">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="92d2f-170">FieldURI</span><span class="sxs-lookup"><span data-stu-id="92d2f-170">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="92d2f-171">Dossiers</span><span class="sxs-lookup"><span data-stu-id="92d2f-171">Folders</span></span>](folders-ex15websvcsotherref.md)
    
<span data-ttu-id="92d2f-172">Pour les codes d’erreur générique à EWS, spécifiques à cette opération, consultez la rubrique [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="92d2f-172">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="92d2f-173">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="92d2f-173">See also</span></span>

- [<span data-ttu-id="92d2f-174">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="92d2f-174">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="92d2f-175">Opération FindFolder</span><span class="sxs-lookup"><span data-stu-id="92d2f-175">FindFolder operation</span></span>](findfolder-operation.md)
    

