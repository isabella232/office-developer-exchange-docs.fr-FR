---
title: GetUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfiguration
api_type:
- schema
ms.assetid: 4044c0a1-cd88-41ae-9cc4-a7cf2b279094
description: L’élément GetUserConfiguration représentent une demande pour obtenir un objet de configuration utilisateur.
ms.openlocfilehash: 81f2ca4995de69d6547412ec699a2ceaddcce385
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827688"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="59e7c-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="59e7c-103">GetUserConfiguration</span></span>

<span data-ttu-id="59e7c-104">L’élément **GetUserConfiguration** représentent une demande pour obtenir un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59e7c-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="59e7c-105">**GetUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="59e7c-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59e7c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59e7c-106">Attributes and elements</span></span>

<span data-ttu-id="59e7c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59e7c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59e7c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="59e7c-108">Attributes</span></span>

<span data-ttu-id="59e7c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59e7c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59e7c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59e7c-110">Child elements</span></span>

|<span data-ttu-id="59e7c-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59e7c-111">**Element**</span></span>|<span data-ttu-id="59e7c-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="59e7c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59e7c-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="59e7c-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="59e7c-114">Représente le nom d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59e7c-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="59e7c-115">Cet élément doit être présent dans une requête GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="59e7c-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="59e7c-116">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="59e7c-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="59e7c-117">Spécifie les types de propriétés de configuration utilisateur à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="59e7c-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="59e7c-118">Cet élément doit être présent dans une requête GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="59e7c-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59e7c-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59e7c-119">Parent elements</span></span>

<span data-ttu-id="59e7c-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59e7c-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="59e7c-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="59e7c-121">Text value</span></span>

<span data-ttu-id="59e7c-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59e7c-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="59e7c-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="59e7c-123">Remarks</span></span>

<span data-ttu-id="59e7c-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="59e7c-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59e7c-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="59e7c-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59e7c-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="59e7c-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59e7c-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="59e7c-127">Schema Name</span></span>  <br/> |<span data-ttu-id="59e7c-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="59e7c-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="59e7c-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="59e7c-129">Validation File</span></span>  <br/> |<span data-ttu-id="59e7c-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="59e7c-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="59e7c-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="59e7c-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="59e7c-132">False</span><span class="sxs-lookup"><span data-stu-id="59e7c-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59e7c-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59e7c-133">See also</span></span>



- [<span data-ttu-id="59e7c-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="59e7c-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

