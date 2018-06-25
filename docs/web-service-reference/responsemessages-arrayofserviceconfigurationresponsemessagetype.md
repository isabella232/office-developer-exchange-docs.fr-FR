---
title: ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessages
api_type:
- schema
ms.assetid: c7cfa0d1-fcb2-441f-8489-3a549da33b34
description: L’élément ResponseMessages contient un tableau de messages de réponse de configuration de service.
ms.openlocfilehash: af8a6db8d6e9d3ec76b532a81ef2a7392dcfde7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829194"
---
# <a name="responsemessages-arrayofserviceconfigurationresponsemessagetype"></a><span data-ttu-id="5c0b6-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="5c0b6-103">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>

<span data-ttu-id="5c0b6-104">L’élément **ResponseMessages** contient un tableau de messages de réponse de configuration de service.</span><span class="sxs-lookup"><span data-stu-id="5c0b6-104">The **ResponseMessages** element contains an array of service configuration response messages.</span></span> 
  
```XML
<ResponseMessages>
   <ServiceConfigurationResponseMessageType/>
</ResponseMessages>
```

 <span data-ttu-id="5c0b6-105">**ArrayOfServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5c0b6-105">**ArrayOfServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c0b6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5c0b6-106">Attributes and elements</span></span>

<span data-ttu-id="5c0b6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5c0b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c0b6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="5c0b6-108">Attributes</span></span>

<span data-ttu-id="5c0b6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5c0b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5c0b6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5c0b6-110">Child elements</span></span>

|<span data-ttu-id="5c0b6-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5c0b6-111">**Element**</span></span>|<span data-ttu-id="5c0b6-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="5c0b6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c0b6-113">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="5c0b6-113">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="5c0b6-114">Contient les paramètres de configuration de service.</span><span class="sxs-lookup"><span data-stu-id="5c0b6-114">Contains service configuration settings.</span></span> <span data-ttu-id="5c0b6-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="5c0b6-115">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c0b6-116">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5c0b6-116">Parent elements</span></span>

|<span data-ttu-id="5c0b6-117">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5c0b6-117">**Element**</span></span>|<span data-ttu-id="5c0b6-118">**Description**</span><span class="sxs-lookup"><span data-stu-id="5c0b6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c0b6-119">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="5c0b6-119">GetServiceConfigurationResponse</span></span>](getserviceconfigurationresponse.md) <br/> |<span data-ttu-id="5c0b6-120">Définit une réponse à une demande de GetServiceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="5c0b6-120">Defines a response to a GetServiceConfiguration request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5c0b6-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="5c0b6-121">Text value</span></span>

<span data-ttu-id="5c0b6-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="5c0b6-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5c0b6-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="5c0b6-123">Remarks</span></span>

<span data-ttu-id="5c0b6-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="5c0b6-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c0b6-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5c0b6-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c0b6-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5c0b6-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c0b6-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5c0b6-127">Schema Name</span></span>  <br/> |<span data-ttu-id="5c0b6-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5c0b6-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5c0b6-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5c0b6-129">Validation File</span></span>  <br/> |<span data-ttu-id="5c0b6-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5c0b6-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c0b6-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5c0b6-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c0b6-132">False</span><span class="sxs-lookup"><span data-stu-id="5c0b6-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c0b6-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5c0b6-133">See also</span></span>



- [<span data-ttu-id="5c0b6-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5c0b6-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

