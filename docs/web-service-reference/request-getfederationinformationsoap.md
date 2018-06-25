---
title: Demande (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: beeb5371-f57b-4346-9753-035dd42c6bee
description: L’élément de demande représente une demande de GetFederationInformationRequest (SOAP).
ms.openlocfilehash: 0fb9301c2f318aa2c27155675dd3c43b41aabecd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829119"
---
# <a name="request-getfederationinformation-soap"></a><span data-ttu-id="2bb17-103">Demande (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2bb17-103">Request (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="2bb17-104">L’élément de **demande** représente une demande de [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="2bb17-104">The **Request** element represents a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) request.</span></span> 
  
```XML
<Request>
   <Domain/>
</Request>
```

 <span data-ttu-id="2bb17-105">**GetFederationInformationRequest**</span><span class="sxs-lookup"><span data-stu-id="2bb17-105">**GetFederationInformationRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2bb17-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2bb17-106">Attributes and elements</span></span>

<span data-ttu-id="2bb17-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2bb17-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2bb17-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2bb17-108">Attributes</span></span>

<span data-ttu-id="2bb17-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2bb17-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2bb17-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2bb17-110">Child elements</span></span>

|<span data-ttu-id="2bb17-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2bb17-111">**Element**</span></span>|<span data-ttu-id="2bb17-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="2bb17-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bb17-113">Domaine (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2bb17-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="2bb17-114">Identifie le domaine qui possède une approbation de fédération.</span><span class="sxs-lookup"><span data-stu-id="2bb17-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2bb17-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2bb17-115">Parent elements</span></span>

|<span data-ttu-id="2bb17-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2bb17-116">**Element**</span></span>|<span data-ttu-id="2bb17-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="2bb17-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2bb17-118">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2bb17-118">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md) <br/> |<span data-ttu-id="2bb17-119">Prépare un appel au serveur pour demander des données de configuration pour le service de jeton de sécurité (STS).</span><span class="sxs-lookup"><span data-stu-id="2bb17-119">Prepares a call to the server to request configuration data for the security token service (STS).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="2bb17-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2bb17-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2bb17-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2bb17-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2bb17-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2bb17-122">Schema Name</span></span>  <br/> |<span data-ttu-id="2bb17-123">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="2bb17-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2bb17-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2bb17-124">Validation File</span></span>  <br/> |<span data-ttu-id="2bb17-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2bb17-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2bb17-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2bb17-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="2bb17-127">True</span><span class="sxs-lookup"><span data-stu-id="2bb17-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2bb17-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2bb17-128">See also</span></span>



[<span data-ttu-id="2bb17-129">Utilisation de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="2bb17-129">Working with Autodiscover</span></span>](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

