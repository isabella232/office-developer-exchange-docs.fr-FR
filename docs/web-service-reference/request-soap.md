---
title: Demande (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75696436-997e-49f1-a31b-eb9a8c3526f3
description: L’élément Request contient les paramètres de configuration demandés et les utilisateurs cibles.
ms.openlocfilehash: 4358713d19e763b75d2a43f147385026f43b1255
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44448988"
---
# <a name="request-soap"></a><span data-ttu-id="353a8-103">Demande (SOAP)</span><span class="sxs-lookup"><span data-stu-id="353a8-103">Request (SOAP)</span></span>

<span data-ttu-id="353a8-104">L’élément **Request** contient les paramètres de configuration demandés et les utilisateurs cibles.</span><span class="sxs-lookup"><span data-stu-id="353a8-104">The **Request** element contains the requested configuration settings and the target users.</span></span> 
  
```XML
<Request>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</Request>
```

 <span data-ttu-id="353a8-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="353a8-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="353a8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="353a8-106">Attributes and elements</span></span>

<span data-ttu-id="353a8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="353a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="353a8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="353a8-108">Attributes</span></span>

<span data-ttu-id="353a8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="353a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="353a8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="353a8-110">Child elements</span></span>

|<span data-ttu-id="353a8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="353a8-111">**Element**</span></span>|<span data-ttu-id="353a8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="353a8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="353a8-113">Utilisateurs (SOAP)</span><span class="sxs-lookup"><span data-stu-id="353a8-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="353a8-114">Représente une collection d’adresses de messagerie des utilisateurs dont les paramètres doivent être récupérés.</span><span class="sxs-lookup"><span data-stu-id="353a8-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="353a8-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="353a8-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="353a8-116">Contient les noms des paramètres de configuration demandés.</span><span class="sxs-lookup"><span data-stu-id="353a8-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="353a8-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="353a8-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="353a8-118">Spécifie la version du serveur spécifique que le fournisseur souhaite utiliser.</span><span class="sxs-lookup"><span data-stu-id="353a8-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="353a8-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="353a8-119">Parent elements</span></span>

|<span data-ttu-id="353a8-120">**Élément**</span><span class="sxs-lookup"><span data-stu-id="353a8-120">**Element**</span></span>|<span data-ttu-id="353a8-121">**Description**</span><span class="sxs-lookup"><span data-stu-id="353a8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="353a8-122">GetUserSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="353a8-122">GetUserSettingsRequestMessage (SOAP)</span></span>](getusersettingsrequestmessage-soap.md) <br/> |<span data-ttu-id="353a8-123">Représente une demande d' [opération GetUserSettings (SOAP)](getusersettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="353a8-123">Represents a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="353a8-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="353a8-124">Text value</span></span>

<span data-ttu-id="353a8-125">Aucune.</span><span class="sxs-lookup"><span data-stu-id="353a8-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="353a8-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="353a8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="353a8-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="353a8-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="353a8-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="353a8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="353a8-129">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="353a8-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="353a8-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="353a8-130">Validation File</span></span>  <br/> |<span data-ttu-id="353a8-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="353a8-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="353a8-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="353a8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="353a8-133">True</span><span class="sxs-lookup"><span data-stu-id="353a8-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="353a8-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="353a8-134">See also</span></span>



[<span data-ttu-id="353a8-135">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="353a8-135">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

