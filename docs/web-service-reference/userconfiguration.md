---
title: UserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserConfiguration
api_type:
- schema
ms.assetid: 1811df99-ca5b-48a3-b160-b3fd70320c34
description: L’élément UserConfiguration définit un objet de configuration utilisateur unique.
ms.openlocfilehash: 1217f5d591570c2d8df49a116b6bf35c243d1e0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468907"
---
# <a name="userconfiguration"></a><span data-ttu-id="d1a82-103">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1a82-103">UserConfiguration</span></span>

<span data-ttu-id="d1a82-104">L’élément **UserConfiguration** définit un objet de configuration utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="d1a82-104">The **UserConfiguration** element defines a single user configuration object.</span></span> 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 <span data-ttu-id="d1a82-105">**UserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="d1a82-105">**UserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1a82-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d1a82-106">Attributes and elements</span></span>

<span data-ttu-id="d1a82-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d1a82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1a82-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d1a82-108">Attributes</span></span>

<span data-ttu-id="d1a82-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d1a82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1a82-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d1a82-110">Child elements</span></span>

|<span data-ttu-id="d1a82-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d1a82-111">**Element**</span></span>|<span data-ttu-id="d1a82-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="d1a82-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1a82-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="d1a82-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="d1a82-114">Représente le nom d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1a82-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="d1a82-115">Cet élément doit être utilisé lors de la création d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1a82-115">This element must be used when you create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="d1a82-116">ItemId</span><span class="sxs-lookup"><span data-stu-id="d1a82-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="d1a82-117">Définit l’identificateur d’élément d’objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1a82-117">Defines the user configuration object item identifier.</span></span>  <br/> |
|[<span data-ttu-id="d1a82-118">Dictionnaire</span><span class="sxs-lookup"><span data-stu-id="d1a82-118">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="d1a82-119">Définit un ensemble d’entrées de propriété de dictionnaire pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1a82-119">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="d1a82-120">XmlData</span><span class="sxs-lookup"><span data-stu-id="d1a82-120">XmlData</span></span>](xmldata.md) <br/> |<span data-ttu-id="d1a82-121">Contient le contenu de propriété de données XML pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1a82-121">Contains XML data property content for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="d1a82-122">BinaryData</span><span class="sxs-lookup"><span data-stu-id="d1a82-122">BinaryData</span></span>](binarydata.md) <br/> |<span data-ttu-id="d1a82-123">Contient le contenu de propriété de données binaires pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1a82-123">Contains binary data property content for a user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d1a82-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d1a82-124">Parent elements</span></span>

|<span data-ttu-id="d1a82-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d1a82-125">**Element**</span></span>|<span data-ttu-id="d1a82-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="d1a82-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1a82-127">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1a82-127">CreateUserConfiguration</span></span>](createuserconfiguration.md) <br/> |<span data-ttu-id="d1a82-128">Représente une demande de création d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1a82-128">Represents a request to create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="d1a82-129">GetUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d1a82-129">GetUserConfigurationResponseMessage</span></span>](getuserconfigurationresponsemessage.md) <br/> |<span data-ttu-id="d1a82-130">Représente une réponse qui retourne un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1a82-130">Represents a response that returns a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="d1a82-131">UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="d1a82-131">UpdateUserConfiguration</span></span>](updateuserconfiguration.md) <br/> |<span data-ttu-id="d1a82-132">Représente une demande de mise à jour d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="d1a82-132">Represents a request to update a user configuration object.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d1a82-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="d1a82-133">Remarks</span></span>

<span data-ttu-id="d1a82-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1a82-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1a82-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d1a82-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1a82-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d1a82-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d1a82-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d1a82-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d1a82-138">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="d1a82-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d1a82-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d1a82-139">Validation File</span></span>  <br/> |<span data-ttu-id="d1a82-140">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d1a82-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d1a82-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d1a82-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1a82-142">False</span><span class="sxs-lookup"><span data-stu-id="d1a82-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1a82-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d1a82-143">See also</span></span>



- [<span data-ttu-id="d1a82-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d1a82-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

