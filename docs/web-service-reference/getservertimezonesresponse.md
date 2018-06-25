---
title: GetServerTimeZonesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZonesResponse
api_type:
- schema
ms.assetid: 97c94d32-10f1-4c3e-ab20-9fd7e8257e50
description: L’élément GetServerTimeZonesResponse définit une réponse à une demande d’opération GetServerTimeZones.
ms.openlocfilehash: 119809076c82ff75a6dd061fc976f861e13f4e57
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827664"
---
# <a name="getservertimezonesresponse"></a><span data-ttu-id="d08f5-103">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="d08f5-103">GetServerTimeZonesResponse</span></span>

<span data-ttu-id="d08f5-104">L’élément **GetServerTimeZonesResponse** définit une réponse à une demande [d’opération GetServerTimeZones](getservertimezones-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="d08f5-104">The **GetServerTimeZonesResponse** element defines a response to a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span> 
  
```XML
<GetServerTimeZonesResponse>
   <ResponseMessages/>
</GetServerTimeZonesResponse>
```

 <span data-ttu-id="d08f5-105">**GetServerTimeZonesResponseType**</span><span class="sxs-lookup"><span data-stu-id="d08f5-105">**GetServerTimeZonesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d08f5-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d08f5-106">Attributes and elements</span></span>

<span data-ttu-id="d08f5-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d08f5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d08f5-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d08f5-108">Attributes</span></span>

<span data-ttu-id="d08f5-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d08f5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d08f5-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d08f5-110">Child elements</span></span>

|<span data-ttu-id="d08f5-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d08f5-111">**Element**</span></span>|<span data-ttu-id="d08f5-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d08f5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d08f5-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d08f5-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d08f5-114">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d08f5-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d08f5-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d08f5-115">Parent elements</span></span>

<span data-ttu-id="d08f5-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d08f5-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d08f5-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="d08f5-117">Remarks</span></span>

<span data-ttu-id="d08f5-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d08f5-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d08f5-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d08f5-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d08f5-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d08f5-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d08f5-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d08f5-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d08f5-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d08f5-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d08f5-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d08f5-123">Validation File</span></span>  <br/> |<span data-ttu-id="d08f5-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d08f5-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d08f5-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d08f5-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d08f5-126">False</span><span class="sxs-lookup"><span data-stu-id="d08f5-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d08f5-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d08f5-127">See also</span></span>



- [<span data-ttu-id="d08f5-128">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d08f5-128">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

