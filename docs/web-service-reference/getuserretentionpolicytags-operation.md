---
title: Opération GetUserRetentionPolicyTags
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57c6ff23-5c2c-42ee-824b-5a1b6dafab8c
description: Opération de recherche plus d’informations sur la GetUserRetentionPolicyTags EWS.
ms.openlocfilehash: faf3553c5dd426b522659029bda6819c55f2708d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353230"
---
# <a name="getuserretentionpolicytags-operation"></a><span data-ttu-id="dcd18-103">Opération GetUserRetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="dcd18-103">GetUserRetentionPolicyTags operation</span></span>

<span data-ttu-id="dcd18-104">Trouvez des informations sur l’opération EWS **GetUserRetentionPolicyTags** .</span><span class="sxs-lookup"><span data-stu-id="dcd18-104">Find information about the **GetUserRetentionPolicyTags** EWS operation.</span></span> 
  
<span data-ttu-id="dcd18-105">L’opération **GetUserRetentionPolicyTags** Obtient une liste de tous les par défaut, dossier système et des balises personnelles qui sont associés à un utilisateur à l’aide d’une stratégie système ou qui ont été appliquées par l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="dcd18-105">The **GetUserRetentionPolicyTags** operation gets a list of all default, system folder, and personal tags that are associated with a user by means of a system policy or that were applied by the user.</span></span> 
  
<span data-ttu-id="dcd18-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="dcd18-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getuserretentionpolicytags-operation"></a><span data-ttu-id="dcd18-107">Utilisation de l’opération GetUserRetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="dcd18-107">Using the GetUserRetentionPolicyTags operation</span></span>

<span data-ttu-id="dcd18-108">Cette opération renvoie le nom complet, ID de rétention, période de rétention, type de rétention, action de rétention et des balises description et les valeurs des propriétés **IsVisible**, **OptedInto**et **IsArchive** .</span><span class="sxs-lookup"><span data-stu-id="dcd18-108">This operation returns the display name, retention ID, retention period, retention type, retention action, and description tags, and the values for the **IsVisible**, **OptedInto**, and **IsArchive** properties.</span></span> 
  
### <a name="getuserretentionpolicytags-operation-soap-headers"></a><span data-ttu-id="dcd18-109">En-têtes SOAP GetUserRetentionPolicyTags opération</span><span class="sxs-lookup"><span data-stu-id="dcd18-109">GetUserRetentionPolicyTags operation SOAP headers</span></span>

<span data-ttu-id="dcd18-110">L’opération **GetUserRetentionPolicyTags** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="dcd18-110">The **GetUserRetentionPolicyTags** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="dcd18-111">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="dcd18-111">**Header name**</span></span>|<span data-ttu-id="dcd18-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dcd18-112">**Element**</span></span>|<span data-ttu-id="dcd18-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="dcd18-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dcd18-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="dcd18-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="dcd18-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="dcd18-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="dcd18-116">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="dcd18-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="dcd18-117">Ceci s’applique à une demande.</span><span class="sxs-lookup"><span data-stu-id="dcd18-117">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="dcd18-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="dcd18-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="dcd18-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="dcd18-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="dcd18-120">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="dcd18-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="dcd18-121">Cela s’applique à une réponse.</span><span class="sxs-lookup"><span data-stu-id="dcd18-121">This is applicable to a response.</span></span>  <br/> |
   
## <a name="getuserretentionpolicytags-operation-request-example"></a><span data-ttu-id="dcd18-122">Exemple de requête d’opération GetUserRetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="dcd18-122">GetUserRetentionPolicyTags operation request example</span></span>

<span data-ttu-id="dcd18-123">Une demande d’opération **GetUserRetentionPolicyTags** l’exemple suivant montre comment obtenir la liste des balises pour l’utilisateur actuel.</span><span class="sxs-lookup"><span data-stu-id="dcd18-123">The following example of a **GetUserRetentionPolicyTags** operation request shows how to get a list of tags for the current user.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetUserRetentionPolicyTags />
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="dcd18-124">La demande SOAP body contienne l’élément suivant :</span><span class="sxs-lookup"><span data-stu-id="dcd18-124">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="dcd18-125">GetUserRetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="dcd18-125">GetUserRetentionPolicyTags</span></span>](getuserretentionpolicytags.md)
    
## <a name="successful-getuserretentionpolicytags-operation-response"></a><span data-ttu-id="dcd18-126">Réponse d’opération GetUserRetentionPolicyTags réussie</span><span class="sxs-lookup"><span data-stu-id="dcd18-126">Successful GetUserRetentionPolicyTags operation response</span></span>

<span data-ttu-id="dcd18-127">L’exemple suivant montre une réponse positive à une demande d’opération **GetUserRetentionPolicyTags** .</span><span class="sxs-lookup"><span data-stu-id="dcd18-127">The following example shows a successful response to a **GetUserRetentionPolicyTags** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="179" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserRetentionPolicyTagsResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <RetentionPolicyTags>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>1 Year Delete</DisplayName>
               <RetentionId>e66252f9-794f-4b36-b55e-d6d95fdf87a3</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>true</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Personal 1 year move to archive</DisplayName>
               <RetentionId>b2a29464-649c-4174-932b-6aaac9811c89</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>MoveToArchive</RetentionAction>
               <Description/>
               <IsVisible>true</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>true</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Sent Items</DisplayName>
               <RetentionId>b0d32f1b-fbd0-4c1d-ba3e-ddd1086ea1d3</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>SentItems</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Default 1 year delete</DisplayName>
               <RetentionId>29fc9b9d-98b0-4c01-acf8-3996e2afce98</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>All</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Two Year Retention</DisplayName>
               <RetentionId>a1a38957-2557-404e-9f32-53d77c948f62</RetentionId>
               <RetentionPeriod>730</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description>Use this tag for all items to be retained for two years.</Description>
               <IsVisible>true</IsVisible>
               <OptedInto>true</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Default two year move to archive</DisplayName>
               <RetentionId>75bc8dbe-a0e8-4e09-9fa3-fd4c21f49318</RetentionId>
               <RetentionPeriod>730</RetentionPeriod>
               <Type>All</Type>
               <RetentionAction>MoveToArchive</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>true</IsArchive>
            </RetentionPolicyTag>
         </RetentionPolicyTags>
      </GetUserRetentionPolicyTagsResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="dcd18-128">La réponse SOAP body contient les éléments suivants :</span><span class="sxs-lookup"><span data-stu-id="dcd18-128">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="dcd18-129">GetUserRetentionPolicyTagsResponse</span><span class="sxs-lookup"><span data-stu-id="dcd18-129">GetUserRetentionPolicyTagsResponse</span></span>](getuserretentionpolicytagsresponse.md)
    
- [<span data-ttu-id="dcd18-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="dcd18-130">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="dcd18-131">RetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="dcd18-131">RetentionPolicyTags</span></span>](retentionpolicytags.md)
    
- [<span data-ttu-id="dcd18-132">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="dcd18-132">RetentionPolicyTag</span></span>](retentionpolicytag.md)
    
- [<span data-ttu-id="dcd18-133">DisplayName (chaîne)</span><span class="sxs-lookup"><span data-stu-id="dcd18-133">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="dcd18-134">RetentionId</span><span class="sxs-lookup"><span data-stu-id="dcd18-134">RetentionId</span></span>](retentionid.md)
    
- [<span data-ttu-id="dcd18-135">RetentionPeriod</span><span class="sxs-lookup"><span data-stu-id="dcd18-135">RetentionPeriod</span></span>](retentionperiod.md)
    
- [<span data-ttu-id="dcd18-136">Type (ElcFolderType)</span><span class="sxs-lookup"><span data-stu-id="dcd18-136">Type (ElcFolderType)</span></span>](type-elcfoldertype.md)
    
- [<span data-ttu-id="dcd18-137">RetentionAction</span><span class="sxs-lookup"><span data-stu-id="dcd18-137">RetentionAction</span></span>](retentionaction.md)
    
- [<span data-ttu-id="dcd18-138">Description</span><span class="sxs-lookup"><span data-stu-id="dcd18-138">Description</span></span>](description.md)
    
- [<span data-ttu-id="dcd18-139">IsVisible</span><span class="sxs-lookup"><span data-stu-id="dcd18-139">IsVisible</span></span>](isvisible.md)
    
- [<span data-ttu-id="dcd18-140">OptedInto</span><span class="sxs-lookup"><span data-stu-id="dcd18-140">OptedInto</span></span>](optedinto.md)
    
- [<span data-ttu-id="dcd18-141">IsArchive</span><span class="sxs-lookup"><span data-stu-id="dcd18-141">IsArchive</span></span>](isarchive.md)
    
## <a name="getuserretentionpolicytags-operation-error-response"></a><span data-ttu-id="dcd18-142">Réponse d’erreur d’opération GetUserRetentionPolicyTags</span><span class="sxs-lookup"><span data-stu-id="dcd18-142">GetUserRetentionPolicyTags operation error response</span></span>

<span data-ttu-id="dcd18-143">Pour les codes d’erreur qui sont génériques pour EWS, voir [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="dcd18-143">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
