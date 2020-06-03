---
title: WebClientUrls (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: fdfe6059-a861-4fa2-a20e-ee6ab820bee9
description: L’élément WebClientUrls représente un paramètre utilisateur qui contient une collection d’éléments WebClientUrl (SOAP).
ms.openlocfilehash: 80c8ab36e30146c78f4bdb4f40eb9f87a335199c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464923"
---
# <a name="webclienturls-soap"></a><span data-ttu-id="ff06f-103">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff06f-103">WebClientUrls (SOAP)</span></span>

<span data-ttu-id="ff06f-104">L’élément **WebClientUrls** représente un paramètre utilisateur qui contient une collection d’éléments [WebClientUrl (SOAP)](webclienturl-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="ff06f-104">The **WebClientUrls** element represents a user setting that contains a collection of [WebClientUrl (SOAP)](webclienturl-soap.md) elements.</span></span> 
  
[<span data-ttu-id="ff06f-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff06f-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="ff06f-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff06f-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="ff06f-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff06f-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrls>
     <WebClientUrl/>
</WebClientUrls>

```

 <span data-ttu-id="ff06f-108">**WebClientUrls**</span><span class="sxs-lookup"><span data-stu-id="ff06f-108">**WebClientUrls**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff06f-109">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ff06f-109">Attributes and elements</span></span>

<span data-ttu-id="ff06f-110">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ff06f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff06f-111">Attributs</span><span class="sxs-lookup"><span data-stu-id="ff06f-111">Attributes</span></span>

<span data-ttu-id="ff06f-112">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ff06f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff06f-113">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ff06f-113">Child elements</span></span>

|<span data-ttu-id="ff06f-114">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ff06f-114">**Element**</span></span>|<span data-ttu-id="ff06f-115">**Description**</span><span class="sxs-lookup"><span data-stu-id="ff06f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff06f-116">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff06f-116">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md) <br/> |<span data-ttu-id="ff06f-117">Représente une URL de client Exchange.</span><span class="sxs-lookup"><span data-stu-id="ff06f-117">Represents an Exchange client URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ff06f-118">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ff06f-118">Parent elements</span></span>

|<span data-ttu-id="ff06f-119">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ff06f-119">**Element**</span></span>|<span data-ttu-id="ff06f-120">**Description**</span><span class="sxs-lookup"><span data-stu-id="ff06f-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff06f-121">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff06f-121">UserSetting (SOAP)</span></span>](usersetting-soap.md) <br/> |<span data-ttu-id="ff06f-122">Représente une réponse à une demande GetUserSettings.</span><span class="sxs-lookup"><span data-stu-id="ff06f-122">Represents a response to a GetUserSettings request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="ff06f-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ff06f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff06f-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ff06f-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="ff06f-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ff06f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="ff06f-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="ff06f-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="ff06f-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ff06f-127">Validation File</span></span>  <br/> |<span data-ttu-id="ff06f-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ff06f-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ff06f-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ff06f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff06f-130">True</span><span class="sxs-lookup"><span data-stu-id="ff06f-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff06f-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ff06f-131">See also</span></span>



[<span data-ttu-id="ff06f-132">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="ff06f-132">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)

