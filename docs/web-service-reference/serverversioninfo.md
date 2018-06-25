---
title: ServerVersionInfo
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServerVersionInfo
api_type:
- schema
ms.assetid: c04a6872-ca27-432b-aac2-36b023d0afc6
description: L’élément ServerVersionInfo représente le numéro de version de Microsoft Exchange Server.
ms.openlocfilehash: aff8a6542e2ae6fb1148dd29051b7b33ad90eeff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829389"
---
# <a name="serverversioninfo"></a><span data-ttu-id="6af61-103">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="6af61-103">ServerVersionInfo</span></span>

<span data-ttu-id="6af61-104">L’élément **ServerVersionInfo** représente le numéro de version de Microsoft Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="6af61-104">The **ServerVersionInfo** element represents the Microsoft Exchange Server version number.</span></span> 
  
```xml
<ServerVersionInfo MajorVersion="" MinorVersion="" MajorBuildNumber="" MinorBuildNumber="" Version="" />
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6af61-105">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6af61-105">Attributes and elements</span></span>

<span data-ttu-id="6af61-106">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6af61-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6af61-107">Attributs</span><span class="sxs-lookup"><span data-stu-id="6af61-107">Attributes</span></span>

|<span data-ttu-id="6af61-108">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="6af61-108">**Attribute**</span></span>|<span data-ttu-id="6af61-109">**Description**</span><span class="sxs-lookup"><span data-stu-id="6af61-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6af61-110">MajorVersion</span><span class="sxs-lookup"><span data-stu-id="6af61-110">MajorVersion</span></span>  <br/> |<span data-ttu-id="6af61-111">Décrit le numéro de version majeur.</span><span class="sxs-lookup"><span data-stu-id="6af61-111">Describes the major version number.</span></span>  <br/> |
|<span data-ttu-id="6af61-112">MinorVersion</span><span class="sxs-lookup"><span data-stu-id="6af61-112">MinorVersion</span></span>  <br/> |<span data-ttu-id="6af61-113">Décrit le numéro de version secondaire.</span><span class="sxs-lookup"><span data-stu-id="6af61-113">Describes the minor version number.</span></span>  <br/> |
|<span data-ttu-id="6af61-114">MajorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="6af61-114">MajorBuildNumber</span></span>  <br/> |<span data-ttu-id="6af61-115">Décrit le numéro de version majeur.</span><span class="sxs-lookup"><span data-stu-id="6af61-115">Describes the major build number.</span></span>  <br/> |
|<span data-ttu-id="6af61-116">MinorBuildNumber</span><span class="sxs-lookup"><span data-stu-id="6af61-116">MinorBuildNumber</span></span>  <br/> |<span data-ttu-id="6af61-117">Décrit le numéro de version secondaire.</span><span class="sxs-lookup"><span data-stu-id="6af61-117">Describes the minor build number.</span></span>  <br/> |
|<span data-ttu-id="6af61-118">Version</span><span class="sxs-lookup"><span data-stu-id="6af61-118">Version</span></span>  <br/> |<span data-ttu-id="6af61-119">Décrit la version du schéma Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="6af61-119">Describes the Exchange Web Services (EWS) schema version.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6af61-120">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6af61-120">Child elements</span></span>

<span data-ttu-id="6af61-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6af61-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6af61-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6af61-122">Parent elements</span></span>

<span data-ttu-id="6af61-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6af61-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6af61-124">Remarques</span><span class="sxs-lookup"><span data-stu-id="6af61-124">Remarks</span></span>

<span data-ttu-id="6af61-125">Cet élément est retourné dans l’en-tête SOAP d’un message de réponse des Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="6af61-125">This element is returned in the SOAP header of an Exchange Web Services response message.</span></span>
  
<span data-ttu-id="6af61-126">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="6af61-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="6af61-127">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6af61-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6af61-128">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6af61-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6af61-129">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6af61-129">Schema Name</span></span>  <br/> |<span data-ttu-id="6af61-130">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="6af61-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="6af61-131">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6af61-131">Validation File</span></span>  <br/> |<span data-ttu-id="6af61-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6af61-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6af61-133">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6af61-133">Can Be Empty</span></span>  <br/> |<span data-ttu-id="6af61-134">False</span><span class="sxs-lookup"><span data-stu-id="6af61-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6af61-135">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6af61-135">See also</span></span>



- [<span data-ttu-id="6af61-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6af61-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

