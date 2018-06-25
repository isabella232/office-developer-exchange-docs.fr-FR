---
title: GetUserSettingsRequest (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 832a9211-d2d5-4a49-bcb3-1dc6dc3904ed
description: L’élément GetUserSettingsRequest représente une demande pour récupérer les paramètres spécifiés pour un ou plusieurs utilisateurs.
ms.openlocfilehash: dc22570144a6947dc6e7042326c7416422680cc1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827702"
---
# <a name="getusersettingsrequest-soap"></a><span data-ttu-id="95422-103">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="95422-103">GetUserSettingsRequest (SOAP)</span></span>

<span data-ttu-id="95422-104">L’élément **GetUserSettingsRequest** représente une demande pour récupérer les paramètres spécifiés pour un ou plusieurs utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="95422-104">The **GetUserSettingsRequest** element represents a request to retrieve specified settings for one or more users.</span></span> 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 <span data-ttu-id="95422-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="95422-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95422-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="95422-106">Attributes and elements</span></span>

<span data-ttu-id="95422-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="95422-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95422-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="95422-108">Attributes</span></span>

<span data-ttu-id="95422-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="95422-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="95422-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="95422-110">Child elements</span></span>

|<span data-ttu-id="95422-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="95422-111">**Element**</span></span>|<span data-ttu-id="95422-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="95422-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95422-113">Utilisateurs (SOAP)</span><span class="sxs-lookup"><span data-stu-id="95422-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="95422-114">Représente une collection d’adresses de messagerie des utilisateurs pour lesquels les paramètres doivent être récupérés.</span><span class="sxs-lookup"><span data-stu-id="95422-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="95422-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="95422-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="95422-116">Contient les noms des paramètres de configuration demandé.</span><span class="sxs-lookup"><span data-stu-id="95422-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="95422-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="95422-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="95422-118">Spécifie la version de serveur spécifique que le fournisseur souhaite utiliser.</span><span class="sxs-lookup"><span data-stu-id="95422-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="95422-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="95422-119">Parent elements</span></span>

<span data-ttu-id="95422-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="95422-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="95422-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="95422-121">Text value</span></span>

<span data-ttu-id="95422-122">Aucun.</span><span class="sxs-lookup"><span data-stu-id="95422-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95422-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="95422-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95422-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="95422-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="95422-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="95422-125">Schema Name</span></span>  <br/> |<span data-ttu-id="95422-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="95422-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="95422-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="95422-127">Validation File</span></span>  <br/> |<span data-ttu-id="95422-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="95422-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="95422-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="95422-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="95422-130">True</span><span class="sxs-lookup"><span data-stu-id="95422-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95422-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="95422-131">See also</span></span>



[<span data-ttu-id="95422-132">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="95422-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

