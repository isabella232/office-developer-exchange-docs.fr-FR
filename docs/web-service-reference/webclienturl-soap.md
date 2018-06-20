---
title: WebClientUrl (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7f8cb6d6-4aac-4a1f-8bec-2dcb90fc1df6
description: L’élément WebClientUrl représente l’URL d’un client web de Exchange.
ms.openlocfilehash: 649845018acee1706a96f9e37475a6d5c5fa0aa7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839038"
---
# <a name="webclienturl-soap"></a><span data-ttu-id="2fbe6-103">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2fbe6-103">WebClientUrl (SOAP)</span></span>

<span data-ttu-id="2fbe6-104">L’élément **WebClientUrl** représente l’URL d’un client web de Exchange.</span><span class="sxs-lookup"><span data-stu-id="2fbe6-104">The **WebClientUrl** element represents the URL of an Exchange web client.</span></span> 
  
[<span data-ttu-id="2fbe6-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2fbe6-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="2fbe6-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2fbe6-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="2fbe6-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2fbe6-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 <span data-ttu-id="2fbe6-108">**WebClientUrl**</span><span class="sxs-lookup"><span data-stu-id="2fbe6-108">**WebClientUrl**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2fbe6-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2fbe6-109">Attributes and elements</span></span>

<span data-ttu-id="2fbe6-110">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2fbe6-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2fbe6-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="2fbe6-111">Attributes</span></span>

<span data-ttu-id="2fbe6-112">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2fbe6-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2fbe6-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2fbe6-113">Child elements</span></span>

|<span data-ttu-id="2fbe6-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2fbe6-114">**Element**</span></span>|<span data-ttu-id="2fbe6-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="2fbe6-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fbe6-116">AuthenticationMethods (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2fbe6-116">AuthenticationMethods (SOAP)</span></span>](authenticationmethods-soap.md) <br/> |<span data-ttu-id="2fbe6-117">Représente la méthode d’authentification pour accéder à l’URL spécifiée.</span><span class="sxs-lookup"><span data-stu-id="2fbe6-117">Represents the authentication method to use when accessing the specified URL.</span></span>  <br/> |
|[<span data-ttu-id="2fbe6-118">URL (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2fbe6-118">Url (SOAP)</span></span>](url-soap.md) <br/> |<span data-ttu-id="2fbe6-119">Représente l’adresse web pour l’URL.</span><span class="sxs-lookup"><span data-stu-id="2fbe6-119">Represents the web address for the URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2fbe6-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2fbe6-120">Parent elements</span></span>

|<span data-ttu-id="2fbe6-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2fbe6-121">**Element**</span></span>|<span data-ttu-id="2fbe6-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="2fbe6-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fbe6-123">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2fbe6-123">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md) <br/> |<span data-ttu-id="2fbe6-124">Représente un paramètre d’utilisateur qui contient une collection d’éléments **WebClientUrl** .</span><span class="sxs-lookup"><span data-stu-id="2fbe6-124">Represents a user setting that contains a collection of **WebClientUrl** elements.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="2fbe6-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2fbe6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2fbe6-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2fbe6-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2fbe6-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2fbe6-127">Schema Name</span></span>  <br/> |<span data-ttu-id="2fbe6-128">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="2fbe6-128">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2fbe6-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2fbe6-129">Validation File</span></span>  <br/> |<span data-ttu-id="2fbe6-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2fbe6-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2fbe6-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2fbe6-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="2fbe6-132">True</span><span class="sxs-lookup"><span data-stu-id="2fbe6-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2fbe6-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2fbe6-133">See also</span></span>



[<span data-ttu-id="2fbe6-134">URL (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2fbe6-134">Url (SOAP)</span></span>](url-soap.md)
  
[<span data-ttu-id="2fbe6-135">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2fbe6-135">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)

