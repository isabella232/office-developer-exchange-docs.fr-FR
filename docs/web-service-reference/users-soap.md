---
title: Utilisateurs (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 4e051617-4eea-47d0-871a-ea1f17a0f711
description: L’élément Users représente une collection d’adresses de messagerie des utilisateurs dont les paramètres doivent être récupérés.
ms.openlocfilehash: 851447a2918e365b7c5d8812a61c9d425d26ffa2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461897"
---
# <a name="users-soap"></a><span data-ttu-id="22d93-103">Utilisateurs (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22d93-103">Users (SOAP)</span></span>

<span data-ttu-id="22d93-104">L’élément **Users** représente une collection d’adresses de messagerie des utilisateurs dont les paramètres doivent être récupérés.</span><span class="sxs-lookup"><span data-stu-id="22d93-104">The **Users** element represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span> 
  
```XML
<Users>
   <User/>
</Users>
```

 <span data-ttu-id="22d93-105">**Utilisateurs**</span><span class="sxs-lookup"><span data-stu-id="22d93-105">**Users**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22d93-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="22d93-106">Attributes and elements</span></span>

<span data-ttu-id="22d93-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="22d93-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22d93-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="22d93-108">Attributes</span></span>

<span data-ttu-id="22d93-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="22d93-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22d93-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="22d93-110">Child elements</span></span>

|<span data-ttu-id="22d93-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22d93-111">**Element**</span></span>|<span data-ttu-id="22d93-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="22d93-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22d93-113">Utilisateur (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22d93-113">User (SOAP)</span></span>](user-soap.md) <br/> |<span data-ttu-id="22d93-114">Représente l’adresse de messagerie d’un utilisateur.</span><span class="sxs-lookup"><span data-stu-id="22d93-114">Represents the e-mail address of a user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22d93-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="22d93-115">Parent elements</span></span>

|<span data-ttu-id="22d93-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="22d93-116">**Element**</span></span>|<span data-ttu-id="22d93-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="22d93-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22d93-118">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22d93-118">GetUserSettingsRequest (SOAP)</span></span>](getusersettingsrequest-soap.md) <br/> |<span data-ttu-id="22d93-119">Représente une demande de récupération des paramètres spécifiés pour un ou plusieurs utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="22d93-119">Represents a request to retrieve specified settings for one or more users.</span></span>  <br/> |
|[<span data-ttu-id="22d93-120">Demande (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22d93-120">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="22d93-121">Contient les paramètres de configuration demandés et les utilisateurs cibles.</span><span class="sxs-lookup"><span data-stu-id="22d93-121">Contains the requested configuration settings and the target users.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="22d93-122">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="22d93-122">Text value</span></span>

<span data-ttu-id="22d93-123">Aucune.</span><span class="sxs-lookup"><span data-stu-id="22d93-123">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22d93-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="22d93-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22d93-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="22d93-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="22d93-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="22d93-126">Schema Name</span></span>  <br/> |<span data-ttu-id="22d93-127">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="22d93-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="22d93-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="22d93-128">Validation File</span></span>  <br/> |<span data-ttu-id="22d93-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="22d93-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="22d93-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="22d93-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="22d93-131">True</span><span class="sxs-lookup"><span data-stu-id="22d93-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="22d93-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="22d93-132">See also</span></span>



[<span data-ttu-id="22d93-133">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="22d93-133">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

