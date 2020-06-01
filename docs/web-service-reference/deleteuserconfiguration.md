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
description: L’élément DeleteUserConfiguration représente une demande de suppression d’un objet de configuration utilisateur.
ms.openlocfilehash: 04668ead48e7c321ed7e91cbbeb67c6154c02283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460756"
---
# <a name="deleteuserconfiguration"></a><span data-ttu-id="1fb2d-103">DeleteUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="1fb2d-103">DeleteUserConfiguration</span></span>

<span data-ttu-id="1fb2d-104">L’élément **DeleteUserConfiguration** représente une demande de suppression d’un objet de configuration utilisateur.</span><span class="sxs-lookup"><span data-stu-id="1fb2d-104">The **DeleteUserConfiguration** element represents a request to delete a user configuration object.</span></span> 
  
```xml
<DeleteUserConfiguration>
   <UserConfigurationName/>
</DeleteUserConfiguration>
```

 <span data-ttu-id="1fb2d-105">**DeleteUserConfigurationType**</span><span class="sxs-lookup"><span data-stu-id="1fb2d-105">**DeleteUserConfigurationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1fb2d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="1fb2d-106">Attributes and elements</span></span>

<span data-ttu-id="1fb2d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="1fb2d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1fb2d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="1fb2d-108">Attributes</span></span>

<span data-ttu-id="1fb2d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="1fb2d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1fb2d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="1fb2d-110">Child elements</span></span>

|<span data-ttu-id="1fb2d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="1fb2d-111">**Element**</span></span>|<span data-ttu-id="1fb2d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="1fb2d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1fb2d-113">UserConfigurationName</span><span class="sxs-lookup"><span data-stu-id="1fb2d-113">UserConfigurationName</span></span>](userconfigurationname.md) <br/> |<span data-ttu-id="1fb2d-114">Représente le nom de l’objet de configuration utilisateur à supprimer.</span><span class="sxs-lookup"><span data-stu-id="1fb2d-114">Represents the name of the user configuration object to delete.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1fb2d-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="1fb2d-115">Parent elements</span></span>

<span data-ttu-id="1fb2d-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1fb2d-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="1fb2d-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="1fb2d-117">Text value</span></span>

<span data-ttu-id="1fb2d-118">Aucun.</span><span class="sxs-lookup"><span data-stu-id="1fb2d-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1fb2d-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="1fb2d-119">Remarks</span></span>

<span data-ttu-id="1fb2d-120">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="1fb2d-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1fb2d-121">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="1fb2d-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1fb2d-122">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="1fb2d-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1fb2d-123">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="1fb2d-123">Schema Name</span></span>  <br/> |<span data-ttu-id="1fb2d-124">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="1fb2d-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1fb2d-125">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="1fb2d-125">Validation File</span></span>  <br/> |<span data-ttu-id="1fb2d-126">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1fb2d-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1fb2d-127">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="1fb2d-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="1fb2d-128">False</span><span class="sxs-lookup"><span data-stu-id="1fb2d-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1fb2d-129">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="1fb2d-129">See also</span></span>

- [<span data-ttu-id="1fb2d-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="1fb2d-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

