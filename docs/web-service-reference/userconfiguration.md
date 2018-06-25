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
ms.openlocfilehash: ce3eaa470ef592c5a8e5a7ef24c377bb2feeca2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838949"
---
# <a name="userconfiguration"></a><span data-ttu-id="59055-103">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="59055-103">UserConfiguration</span></span>

<span data-ttu-id="59055-104">L’élément **UserConfiguration** définit un objet de configuration utilisateur unique.</span><span class="sxs-lookup"><span data-stu-id="59055-104">The **UserConfiguration** element defines a single user configuration object.</span></span> 
  
```XML
<UserConfiguration>
   <UserConfigurationName/>
   <ItemId/>
   <Dictionary/>
   <XmlData/>
  <BinaryData/>
</UserConfiguration>
```

 <span data-ttu-id="59055-105">**UserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="59055-105">**UserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59055-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="59055-106">Attributes and elements</span></span>

<span data-ttu-id="59055-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="59055-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59055-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="59055-108">Attributes</span></span>

<span data-ttu-id="59055-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="59055-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59055-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="59055-110">Child elements</span></span>

|<span data-ttu-id="59055-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59055-111">**Element**</span></span>|<span data-ttu-id="59055-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="59055-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59055-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="59055-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="59055-114">Représente le nom d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59055-114">Represents the name of a user configuration object.</span></span> <span data-ttu-id="59055-115">Cet élément doit être utilisé lorsque vous créez un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59055-115">This element must be used when you create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="59055-116">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="59055-116">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="59055-117">Définit l’identificateur d’élément objet configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59055-117">Defines the user configuration object item identifier.</span></span>  <br/> |
|[<span data-ttu-id="59055-118">Dictionnaire</span><span class="sxs-lookup"><span data-stu-id="59055-118">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="59055-119">Définit un ensemble d’entrées de dictionnaire de propriétés pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59055-119">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="59055-120">XmlData</span><span class="sxs-lookup"><span data-stu-id="59055-120">XmlData</span></span>](xmldata.md) <br/> |<span data-ttu-id="59055-121">Contient le contenu de propriété de données XML pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59055-121">Contains XML data property content for a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="59055-122">BinaryData</span><span class="sxs-lookup"><span data-stu-id="59055-122">BinaryData</span></span>](binarydata.md) <br/> |<span data-ttu-id="59055-123">Contient des données binaires propriété pour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59055-123">Contains binary data property content for a user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59055-124">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="59055-124">Parent elements</span></span>

|<span data-ttu-id="59055-125">**Élément**</span><span class="sxs-lookup"><span data-stu-id="59055-125">**Element**</span></span>|<span data-ttu-id="59055-126">**Description**</span><span class="sxs-lookup"><span data-stu-id="59055-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59055-127">CreateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="59055-127">CreateUserConfiguration</span></span>](createuserconfiguration.md) <br/> |<span data-ttu-id="59055-128">Représente une demande pour créer un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59055-128">Represents a request to create a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="59055-129">GetUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="59055-129">GetUserConfigurationResponseMessage</span></span>](getuserconfigurationresponsemessage.md) <br/> |<span data-ttu-id="59055-130">Représente une réponse qui renvoie un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59055-130">Represents a response that returns a user configuration object.</span></span>  <br/> |
|[<span data-ttu-id="59055-131">UpdateUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="59055-131">UpdateUserConfiguration</span></span>](updateuserconfiguration.md) <br/> |<span data-ttu-id="59055-132">Représente une demande pour mettre à jour un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="59055-132">Represents a request to update a user configuration object.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59055-133">Remarques</span><span class="sxs-lookup"><span data-stu-id="59055-133">Remarks</span></span>

<span data-ttu-id="59055-134">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="59055-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59055-135">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="59055-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59055-136">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="59055-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59055-137">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="59055-137">Schema Name</span></span>  <br/> |<span data-ttu-id="59055-138">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="59055-138">Messages schema</span></span>  <br/> |
|<span data-ttu-id="59055-139">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="59055-139">Validation File</span></span>  <br/> |<span data-ttu-id="59055-140">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="59055-140">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="59055-141">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="59055-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="59055-142">False</span><span class="sxs-lookup"><span data-stu-id="59055-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59055-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="59055-143">See also</span></span>



- [<span data-ttu-id="59055-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="59055-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

