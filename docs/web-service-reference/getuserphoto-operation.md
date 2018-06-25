---
title: Opération GetUserPhoto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e
description: Opération de recherche plus d’informations sur la GetUserPhoto EWS.
ms.openlocfilehash: 4465ac7115d96f5b6ef39e467663c9bf1c70e99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827694"
---
# <a name="getuserphoto-operation"></a><span data-ttu-id="c682e-103">Opération GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="c682e-103">GetUserPhoto operation</span></span>

<span data-ttu-id="c682e-104">Trouvez des informations sur l’opération EWS **GetUserPhoto** .</span><span class="sxs-lookup"><span data-stu-id="c682e-104">Find information about the **GetUserPhoto** EWS operation.</span></span> 
  
<span data-ttu-id="c682e-105">L’opération **GetUserPhoto** Obtient une photo de l’utilisateur des Services de domaine Active Directory (AD DS).</span><span class="sxs-lookup"><span data-stu-id="c682e-105">The **GetUserPhoto** operation gets a user photo from Active Directory Domain Services (AD DS).</span></span> 
  
<span data-ttu-id="c682e-106">Cette opération est une nouveauté d’Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c682e-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getuserphoto-operation"></a><span data-ttu-id="c682e-107">Utilisation de l’opération GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="c682e-107">Using the GetUserPhoto operation</span></span>

<span data-ttu-id="c682e-108">L’opération **RemoveContactFromImList** est une opération simple qui accepte une adresse de messagerie d’un utilisateur et la taille de photo demandé et retourne le flux de photos dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="c682e-108">The **RemoveContactFromImList** operation is a simple operation that accepts a user's email address and the requested photo size and returns the photo stream in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c682e-109">EWS dispose d’un SOAP et une opération basée sur REST pour obtenir les photos de l’utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c682e-109">EWS has both a SOAP and a REST-based operation to get user photos.</span></span> <span data-ttu-id="c682e-110">Pour plus d’informations sur l’interface REST, voir [obtenir les photos de l’utilisateur à l’aide de EWS dans Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="c682e-110">For information about the REST interface, see [Get user photos by using EWS in Exchange](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx).</span></span> 
  
### <a name="getuserphoto-operation-soap-headers"></a><span data-ttu-id="c682e-111">En-têtes SOAP GetUserPhoto opération</span><span class="sxs-lookup"><span data-stu-id="c682e-111">GetUserPhoto operation SOAP headers</span></span>

<span data-ttu-id="c682e-112">L’opération **GetUserPhoto** permettre utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="c682e-112">The **GetUserPhoto** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="c682e-113">**Nom de l'en-tête**</span><span class="sxs-lookup"><span data-stu-id="c682e-113">**Header name**</span></span>|<span data-ttu-id="c682e-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c682e-114">**Element**</span></span>|<span data-ttu-id="c682e-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="c682e-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c682e-116">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="c682e-116">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="c682e-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c682e-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c682e-118">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="c682e-118">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="c682e-119">Cet en-tête est applicable à une demande.</span><span class="sxs-lookup"><span data-stu-id="c682e-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c682e-120">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="c682e-120">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="c682e-121">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c682e-121">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c682e-122">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="c682e-122">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="c682e-123">Cet en-tête est applicable à une réponse.</span><span class="sxs-lookup"><span data-stu-id="c682e-123">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getuserphoto-operation-request-example-get-a-users-photo"></a><span data-ttu-id="c682e-124">Exemple de requête d’opération GetUserPhoto : obtenir la photo d’un utilisateur</span><span class="sxs-lookup"><span data-stu-id="c682e-124">GetUserPhoto operation request example: Get a user's photo</span></span>

<span data-ttu-id="c682e-125">Une demande d’opération **GetUserPhoto** l’exemple suivant montre comment obtenir la photo d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c682e-125">The following example of a **GetUserPhoto** operation request shows how to get a user's photo.</span></span> <span data-ttu-id="c682e-126">Cet exemple demande une photo de l’utilisateur qui est de 48 x 48 pixels.</span><span class="sxs-lookup"><span data-stu-id="c682e-126">This example requests a user photo that is 48x48 pixels.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>user1@contoso.com</m:Email>
         <m:SizeRequested>HR48x48</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c682e-127">Les éléments suivants sont utilisés dans la demande SOAP body :</span><span class="sxs-lookup"><span data-stu-id="c682e-127">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="c682e-128">GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="c682e-128">GetUserPhoto</span></span>](getuserphoto.md)
    
- [<span data-ttu-id="c682e-129">Courrier électronique (chaîne)</span><span class="sxs-lookup"><span data-stu-id="c682e-129">Email (String)</span></span>](email-string.md)
    
- [<span data-ttu-id="c682e-130">SizeRequested</span><span class="sxs-lookup"><span data-stu-id="c682e-130">SizeRequested</span></span>](sizerequested.md)
    
## <a name="successful-getuserphoto-operation-response"></a><span data-ttu-id="c682e-131">Réponse d’opération GetUserPhoto réussie</span><span class="sxs-lookup"><span data-stu-id="c682e-131">Successful GetUserPhoto operation response</span></span>

<span data-ttu-id="c682e-132">L’exemple suivant montre une réponse positive à une opération **GetUserPhoto** pour obtenir la photo d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="c682e-132">The following example shows a successful response to a **GetUserPhoto** operation to get a user's photo.</span></span> 
  
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
      <GetUserPhotoResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <HasChanged>true</HasChanged>
         <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/02</PictureData>
      </GetUserPhotoResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="c682e-133">Les éléments suivants sont utilisés dans la réponse SOAP body :</span><span class="sxs-lookup"><span data-stu-id="c682e-133">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="c682e-134">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="c682e-134">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
- [<span data-ttu-id="c682e-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c682e-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c682e-136">HasChanged</span><span class="sxs-lookup"><span data-stu-id="c682e-136">HasChanged</span></span>](haschanged.md)
    
- [<span data-ttu-id="c682e-137">GetUserPhotoResponse</span><span class="sxs-lookup"><span data-stu-id="c682e-137">GetUserPhotoResponse</span></span>](getuserphotoresponse.md)
    
## <a name="getuserphoto-operation-error-response"></a><span data-ttu-id="c682e-138">Réponse d’erreur d’opération GetUserPhoto</span><span class="sxs-lookup"><span data-stu-id="c682e-138">GetUserPhoto operation error response</span></span>

<span data-ttu-id="c682e-139">L’enveloppe SOAP ne renvoie un code d’erreur si une tentative est effectuée pour obtenir une photo de l’utilisateur pour une adresse de messagerie qui n’existe pas dans l’organisation.</span><span class="sxs-lookup"><span data-stu-id="c682e-139">The SOAP envelope will not return an error code if an attempt is made to get a user photo for an email address that doesn't exist in the organization.</span></span> <span data-ttu-id="c682e-140">Un code d’état HTTP 500 s’afficheront dans la réponse pour indiquer que la demande a échoué.</span><span class="sxs-lookup"><span data-stu-id="c682e-140">A 500 HTTP status code will be returned in the response to indicate that the request was unsuccessful.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="c682e-141">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c682e-141">See also</span></span>

- [<span data-ttu-id="c682e-142">Opérations EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c682e-142">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)   
- [<span data-ttu-id="c682e-143">Obtenir les photos de l’utilisateur à l’aide de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c682e-143">Get user photos by using EWS in Exchange</span></span>](http://msdn.microsoft.com/library/f86d1099-1f57-47dc-abf2-4d5ae4e900a9%28Office.15%29.aspx)
    

