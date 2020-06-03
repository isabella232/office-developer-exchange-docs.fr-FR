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
description: L’élément GetUserConfiguration représente une demande d’obtention d’un objet de configuration utilisateur.
ms.openlocfilehash: 46a2a5ebbabfc038692a5de83e0a960e05295061
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457710"
---
# <a name="getuserconfiguration"></a><span data-ttu-id="ec190-103">GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec190-103">GetUserConfiguration</span></span>

<span data-ttu-id="ec190-104">L’élément **GetUserConfiguration** représente une demande d’obtention d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ec190-104">The **GetUserConfiguration** element represent a request to get a user configuration object.</span></span> 
  
```XML
<GetUserConfiguration>
   <UserConfigurationName/>
   <UserConfigurationProperties/>
</GetUserConfiguration>
```

 <span data-ttu-id="ec190-105">**GetUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="ec190-105">**GetUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ec190-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ec190-106">Attributes and elements</span></span>

<span data-ttu-id="ec190-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ec190-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ec190-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ec190-108">Attributes</span></span>

<span data-ttu-id="ec190-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ec190-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ec190-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ec190-110">Child elements</span></span>

|<span data-ttu-id="ec190-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ec190-111">**Element**</span></span>|<span data-ttu-id="ec190-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ec190-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ec190-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="ec190-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="ec190-114">Représente le nom d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ec190-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="ec190-115">Cet élément doit être présent dans une requête GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ec190-115">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
|[<span data-ttu-id="ec190-116">UserConfigurationProperties</span><span class="sxs-lookup"><span data-stu-id="ec190-116">UserConfigurationProperties</span></span>](userconfigurationproperties.md) <br/> |<span data-ttu-id="ec190-117">Spécifie les types de propriétés de configuration de l’utilisateur à renvoyer.</span><span class="sxs-lookup"><span data-stu-id="ec190-117">Specifies the user configuration property types to return.</span></span> <span data-ttu-id="ec190-118">Cet élément doit être présent dans une requête GetUserConfiguration.</span><span class="sxs-lookup"><span data-stu-id="ec190-118">This element must be present in a GetUserConfiguration request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ec190-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ec190-119">Parent elements</span></span>

<span data-ttu-id="ec190-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec190-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ec190-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ec190-121">Text value</span></span>

<span data-ttu-id="ec190-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ec190-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ec190-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="ec190-123">Remarks</span></span>

<span data-ttu-id="ec190-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ec190-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ec190-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ec190-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ec190-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ec190-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ec190-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ec190-127">Schema Name</span></span>  <br/> |<span data-ttu-id="ec190-128">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ec190-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ec190-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ec190-129">Validation File</span></span>  <br/> |<span data-ttu-id="ec190-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ec190-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ec190-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ec190-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="ec190-132">False</span><span class="sxs-lookup"><span data-stu-id="ec190-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ec190-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ec190-133">See also</span></span>



- [<span data-ttu-id="ec190-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ec190-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

