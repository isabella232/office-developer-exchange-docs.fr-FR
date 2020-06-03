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
description: L’élément GetUserSettingsRequest représente une demande de récupération des paramètres spécifiés pour un ou plusieurs utilisateurs.
ms.openlocfilehash: 353facb5d0bbf922a23b33cbaf6f9d2e7d82bd6b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530161"
---
# <a name="getusersettingsrequest-soap"></a><span data-ttu-id="cea16-103">GetUserSettingsRequest (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cea16-103">GetUserSettingsRequest (SOAP)</span></span>

<span data-ttu-id="cea16-104">L’élément **GetUserSettingsRequest** représente une demande de récupération des paramètres spécifiés pour un ou plusieurs utilisateurs.</span><span class="sxs-lookup"><span data-stu-id="cea16-104">The **GetUserSettingsRequest** element represents a request to retrieve specified settings for one or more users.</span></span> 
  
```XML
<GetUserSettingsRequest>
   <Users/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetUserSettingsRequest>
```

 <span data-ttu-id="cea16-105">**GetUserSettingsRequest**</span><span class="sxs-lookup"><span data-stu-id="cea16-105">**GetUserSettingsRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cea16-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="cea16-106">Attributes and elements</span></span>

<span data-ttu-id="cea16-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="cea16-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cea16-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="cea16-108">Attributes</span></span>

<span data-ttu-id="cea16-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cea16-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cea16-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="cea16-110">Child elements</span></span>

|<span data-ttu-id="cea16-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="cea16-111">**Element**</span></span>|<span data-ttu-id="cea16-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="cea16-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cea16-113">Utilisateurs (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cea16-113">Users (SOAP)</span></span>](users-soap.md) <br/> |<span data-ttu-id="cea16-114">Représente une collection d’adresses de messagerie des utilisateurs dont les paramètres doivent être récupérés.</span><span class="sxs-lookup"><span data-stu-id="cea16-114">Represents a collection of e-mail addresses of the users for whom settings should be retrieved.</span></span>  <br/> |
|[<span data-ttu-id="cea16-115">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cea16-115">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md) <br/> |<span data-ttu-id="cea16-116">Contient les noms des paramètres de configuration demandés.</span><span class="sxs-lookup"><span data-stu-id="cea16-116">Contains the names of the requested configuration settings.</span></span>  <br/> |
|[<span data-ttu-id="cea16-117">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cea16-117">RequestedVersion (SOAP)</span></span>](requestedversion-soap.md) <br/> |<span data-ttu-id="cea16-118">Spécifie la version du serveur spécifique que le fournisseur souhaite utiliser.</span><span class="sxs-lookup"><span data-stu-id="cea16-118">Specifies the specific server version that the provider would like to use.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cea16-119">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="cea16-119">Parent elements</span></span>

<span data-ttu-id="cea16-120">Aucun.</span><span class="sxs-lookup"><span data-stu-id="cea16-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="cea16-121">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="cea16-121">Text value</span></span>

<span data-ttu-id="cea16-122">Aucune.</span><span class="sxs-lookup"><span data-stu-id="cea16-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cea16-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="cea16-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cea16-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="cea16-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="cea16-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="cea16-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cea16-126">Schéma de découverte automatique</span><span class="sxs-lookup"><span data-stu-id="cea16-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="cea16-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="cea16-127">Validation File</span></span>  <br/> |<span data-ttu-id="cea16-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cea16-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cea16-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="cea16-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="cea16-130">True</span><span class="sxs-lookup"><span data-stu-id="cea16-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cea16-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="cea16-131">See also</span></span>



[<span data-ttu-id="cea16-132">Opération GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cea16-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

