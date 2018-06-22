---
title: DeleteUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfiguration
api_type:
- schema
ms.assetid: 91b18b6a-d904-476c-996d-b041e859da1e
description: L’élément DeleteUserConfiguration représente une demande pour supprimer un objet de configuration utilisateur.
ms.openlocfilehash: e357c32f95cddc866b77b6f1172ab260837b061b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755873"
---
# <a name="deleteuserconfiguration"></a><span data-ttu-id="ca12a-103">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="ca12a-103">DeleteUserConfiguration</span></span>

<span data-ttu-id="ca12a-104">L’élément **DeleteUserConfiguration** représente une demande pour supprimer un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="ca12a-104">The **DeleteUserConfiguration** element represents a request to delete a user configuration object.</span></span> 
  
```xml
<DeleteUserConfiguration>
   <UserConfigurationName/>
</DeleteUserConfiguration>
```

 <span data-ttu-id="ca12a-105">**DeleteUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="ca12a-105">**DeleteUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ca12a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ca12a-106">Attributes and elements</span></span>

<span data-ttu-id="ca12a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ca12a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ca12a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ca12a-108">Attributes</span></span>

<span data-ttu-id="ca12a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca12a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ca12a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ca12a-110">Child elements</span></span>

|<span data-ttu-id="ca12a-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ca12a-111">**Element**</span></span>|<span data-ttu-id="ca12a-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="ca12a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ca12a-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="ca12a-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="ca12a-114">Représente le nom de l’objet de configuration d’utilisateur à supprimer.</span><span class="sxs-lookup"><span data-stu-id="ca12a-114">Represents the name of the user configuration object to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ca12a-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ca12a-115">Parent elements</span></span>

<span data-ttu-id="ca12a-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca12a-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="ca12a-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="ca12a-117">Text value</span></span>

<span data-ttu-id="ca12a-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ca12a-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ca12a-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="ca12a-119">Remarks</span></span>

<span data-ttu-id="ca12a-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="ca12a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ca12a-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ca12a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ca12a-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ca12a-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ca12a-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ca12a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="ca12a-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ca12a-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ca12a-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ca12a-125">Validation File</span></span>  <br/> |<span data-ttu-id="ca12a-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ca12a-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ca12a-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ca12a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="ca12a-128">False</span><span class="sxs-lookup"><span data-stu-id="ca12a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ca12a-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ca12a-129">See also</span></span>

- [<span data-ttu-id="ca12a-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ca12a-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

