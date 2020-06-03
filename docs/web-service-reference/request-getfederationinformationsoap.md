---
title: Request (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: beeb5371-f57b-4346-9753-035dd42c6bee
description: L’élément Request représente une demande GetFederationInformationRequest (SOAP).
ms.openlocfilehash: dbd88537d03f6325cf0025d08c63ae486544d705
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459580"
---
# <a name="request-getfederationinformation-soap"></a><span data-ttu-id="eae10-103">Request (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eae10-103">Request (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="eae10-104">L’élément **Request** représente une demande [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="eae10-104">The **Request** element represents a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) request.</span></span> 
  
```XML
<Request>
   <Domain/>
</Request>
```

 <span data-ttu-id="eae10-105">**GetFederationInformationRequest**</span><span class="sxs-lookup"><span data-stu-id="eae10-105">**GetFederationInformationRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eae10-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="eae10-106">Attributes and elements</span></span>

<span data-ttu-id="eae10-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="eae10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eae10-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="eae10-108">Attributes</span></span>

<span data-ttu-id="eae10-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="eae10-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eae10-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="eae10-110">Child elements</span></span>

|<span data-ttu-id="eae10-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eae10-111">**Element**</span></span>|<span data-ttu-id="eae10-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="eae10-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eae10-113">Domaine (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eae10-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="eae10-114">Identifie le domaine qui a une approbation de Fédération.</span><span class="sxs-lookup"><span data-stu-id="eae10-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eae10-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="eae10-115">Parent elements</span></span>

|<span data-ttu-id="eae10-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="eae10-116">**Element**</span></span>|<span data-ttu-id="eae10-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="eae10-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eae10-118">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="eae10-118">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md) <br/> |<span data-ttu-id="eae10-119">Prépare un appel au serveur pour demander des données de configuration pour le service d’émission de jeton de sécurité (STS).</span><span class="sxs-lookup"><span data-stu-id="eae10-119">Prepares a call to the server to request configuration data for the security token service (STS).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="eae10-120">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="eae10-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eae10-121">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="eae10-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="eae10-122">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="eae10-122">Schema Name</span></span>  <br/> |<span data-ttu-id="eae10-123">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="eae10-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="eae10-124">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="eae10-124">Validation File</span></span>  <br/> |<span data-ttu-id="eae10-125">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="eae10-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eae10-126">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="eae10-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="eae10-127">True</span><span class="sxs-lookup"><span data-stu-id="eae10-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eae10-128">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="eae10-128">See also</span></span>



[<span data-ttu-id="eae10-129">Utilisation de la découverte automatique</span><span class="sxs-lookup"><span data-stu-id="eae10-129">Working with Autodiscover</span></span>](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

