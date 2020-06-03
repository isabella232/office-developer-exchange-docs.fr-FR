---
title: AnonymousAccessAllowed (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: bf819a65-30f2-4881-a34f-cb30a9c2b6a7
description: L’élément AnonymousAccessAllowed indique si un emplacement de partage de documents nécessite un utilisateur authentifié.
ms.openlocfilehash: b3ff22fbba603bbd74dc08a0dbb1d8687714fe7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466079"
---
# <a name="anonymousaccessallowed-soap"></a><span data-ttu-id="67bf8-103">AnonymousAccessAllowed (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67bf8-103">AnonymousAccessAllowed (SOAP)</span></span>

<span data-ttu-id="67bf8-104">L’élément **AnonymousAccessAllowed** indique si un emplacement de partage de documents nécessite un utilisateur authentifié.</span><span class="sxs-lookup"><span data-stu-id="67bf8-104">The **AnonymousAccessAllowed** element indicates whether a document sharing location requires an authenticated user.</span></span> 
  
```XML
<AnonymousAccessAllowed /> 
```

 <span data-ttu-id="67bf8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="67bf8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67bf8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="67bf8-106">Attributes and elements</span></span>

<span data-ttu-id="67bf8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="67bf8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67bf8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="67bf8-108">Attributes</span></span>

<span data-ttu-id="67bf8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="67bf8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67bf8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="67bf8-110">Child elements</span></span>

<span data-ttu-id="67bf8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="67bf8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="67bf8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="67bf8-112">Parent elements</span></span>

|<span data-ttu-id="67bf8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="67bf8-113">**Element**</span></span>|<span data-ttu-id="67bf8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="67bf8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67bf8-115">DocumentSharingLocation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67bf8-115">DocumentSharingLocation (SOAP)</span></span>](documentsharinglocation-soap.md) <br/> |<span data-ttu-id="67bf8-116">Représente les informations d’emplacement et de métadonnées pour un emplacement de partage de documents.</span><span class="sxs-lookup"><span data-stu-id="67bf8-116">Represents location and metadata information for a document sharing location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="67bf8-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="67bf8-117">Text value</span></span>

<span data-ttu-id="67bf8-118">La valeur booléenne de l’élément **AnonymousAccessAllowed** indique si l’emplacement de partage nécessite un utilisateur authentifié.</span><span class="sxs-lookup"><span data-stu-id="67bf8-118">The Boolean value of the **AnonymousAccessAllowed** element indicates whether the sharing location requires an authenticated user.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="67bf8-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="67bf8-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67bf8-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="67bf8-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="67bf8-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="67bf8-121">Schema Name</span></span>  <br/> |<span data-ttu-id="67bf8-122">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="67bf8-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="67bf8-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="67bf8-123">Validation File</span></span>  <br/> |<span data-ttu-id="67bf8-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="67bf8-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="67bf8-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="67bf8-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="67bf8-126">True</span><span class="sxs-lookup"><span data-stu-id="67bf8-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67bf8-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="67bf8-127">See also</span></span>

- [<span data-ttu-id="67bf8-128">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="67bf8-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="67bf8-129">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="67bf8-129">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="67bf8-130">Éléments XML de découverte automatique SOAP pour Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="67bf8-130">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

