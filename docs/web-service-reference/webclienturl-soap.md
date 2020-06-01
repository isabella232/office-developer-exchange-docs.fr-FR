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
description: L’élément WebClientUrl représente l’URL d’un client Web Exchange.
ms.openlocfilehash: bcf9c8d4fe80de8af4c9500e5e850558a8451d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464972"
---
# <a name="webclienturl-soap"></a><span data-ttu-id="dcc66-103">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dcc66-103">WebClientUrl (SOAP)</span></span>

<span data-ttu-id="dcc66-104">L’élément **WebClientUrl** représente l’URL d’un client Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="dcc66-104">The **WebClientUrl** element represents the URL of an Exchange web client.</span></span> 
  
[<span data-ttu-id="dcc66-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dcc66-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="dcc66-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dcc66-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="dcc66-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dcc66-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 <span data-ttu-id="dcc66-108">**WebClientUrl**</span><span class="sxs-lookup"><span data-stu-id="dcc66-108">**WebClientUrl**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dcc66-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dcc66-109">Attributes and elements</span></span>

<span data-ttu-id="dcc66-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dcc66-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcc66-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="dcc66-111">Attributes</span></span>

<span data-ttu-id="dcc66-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="dcc66-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dcc66-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dcc66-113">Child elements</span></span>

|<span data-ttu-id="dcc66-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dcc66-114">**Element**</span></span>|<span data-ttu-id="dcc66-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="dcc66-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcc66-116">AuthenticationMethods (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dcc66-116">AuthenticationMethods (SOAP)</span></span>](authenticationmethods-soap.md) <br/> |<span data-ttu-id="dcc66-117">Représente la méthode d’authentification à utiliser lors de l’accès à l’URL spécifiée.</span><span class="sxs-lookup"><span data-stu-id="dcc66-117">Represents the authentication method to use when accessing the specified URL.</span></span>  <br/> |
|[<span data-ttu-id="dcc66-118">URL (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dcc66-118">Url (SOAP)</span></span>](url-soap.md) <br/> |<span data-ttu-id="dcc66-119">Représente l’adresse Web de l’URL.</span><span class="sxs-lookup"><span data-stu-id="dcc66-119">Represents the web address for the URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dcc66-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dcc66-120">Parent elements</span></span>

|<span data-ttu-id="dcc66-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dcc66-121">**Element**</span></span>|<span data-ttu-id="dcc66-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="dcc66-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcc66-123">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dcc66-123">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md) <br/> |<span data-ttu-id="dcc66-124">Représente un paramètre utilisateur qui contient une collection d’éléments **WebClientUrl** .</span><span class="sxs-lookup"><span data-stu-id="dcc66-124">Represents a user setting that contains a collection of **WebClientUrl** elements.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="dcc66-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dcc66-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcc66-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dcc66-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="dcc66-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dcc66-127">Schema Name</span></span>  <br/> |<span data-ttu-id="dcc66-128">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="dcc66-128">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="dcc66-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dcc66-129">Validation File</span></span>  <br/> |<span data-ttu-id="dcc66-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dcc66-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dcc66-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dcc66-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="dcc66-132">True</span><span class="sxs-lookup"><span data-stu-id="dcc66-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dcc66-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dcc66-133">See also</span></span>



[<span data-ttu-id="dcc66-134">URL (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dcc66-134">Url (SOAP)</span></span>](url-soap.md)
  
[<span data-ttu-id="dcc66-135">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="dcc66-135">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)

