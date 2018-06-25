---
title: Action (SetClientExtensionActionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: L’élément Action contient l’action que le serveur Exchange doit effectuer sur une application.
ms.openlocfilehash: a231cedfa6e4759dabfcbecfbe9a9b851f834247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755157"
---
# <a name="action-setclientextensionactiontype"></a><span data-ttu-id="b1cac-103">Action (SetClientExtensionActionType)</span><span class="sxs-lookup"><span data-stu-id="b1cac-103">Action (SetClientExtensionActionType)</span></span>

<span data-ttu-id="b1cac-104">L’élément **Action** contient l’action que le serveur Exchange doit effectuer sur une application.</span><span class="sxs-lookup"><span data-stu-id="b1cac-104">The **Action** element contains the action that the Exchange server should take on an app.</span></span> 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 <span data-ttu-id="b1cac-105">**SetClientExtensionActionType**</span><span class="sxs-lookup"><span data-stu-id="b1cac-105">**SetClientExtensionActionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1cac-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b1cac-106">Attributes and elements</span></span>

<span data-ttu-id="b1cac-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b1cac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1cac-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b1cac-108">Attributes</span></span>

|<span data-ttu-id="b1cac-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b1cac-109">**Attribute**</span></span>|<span data-ttu-id="b1cac-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="b1cac-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b1cac-111">ActionId</span><span class="sxs-lookup"><span data-stu-id="b1cac-111">ActionId</span></span>  <br/> |<span data-ttu-id="b1cac-112">Spécifie l’identificateur de l’action.</span><span class="sxs-lookup"><span data-stu-id="b1cac-112">Specifies the identifier of the action.</span></span> <span data-ttu-id="b1cac-113">Cet attribut est requis.</span><span class="sxs-lookup"><span data-stu-id="b1cac-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="b1cac-114">ID ExtensionId</span><span class="sxs-lookup"><span data-stu-id="b1cac-114">ExtensionId</span></span>  <br/> |<span data-ttu-id="b1cac-115">Spécifie l’identificateur de l’extension.</span><span class="sxs-lookup"><span data-stu-id="b1cac-115">Specifies the identifier of the extension.</span></span> <span data-ttu-id="b1cac-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="b1cac-116">This attribute is optional.</span></span>  <br/> |
   
#### <a name="actionid"></a><span data-ttu-id="b1cac-117">ActionId</span><span class="sxs-lookup"><span data-stu-id="b1cac-117">ActionId</span></span>

|<span data-ttu-id="b1cac-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="b1cac-118">**Value**</span></span>|<span data-ttu-id="b1cac-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="b1cac-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b1cac-120">Configurer</span><span class="sxs-lookup"><span data-stu-id="b1cac-120">Configure</span></span>  <br/> |<span data-ttu-id="b1cac-121">Indique une action de configuration.</span><span class="sxs-lookup"><span data-stu-id="b1cac-121">Indicates a configuration action.</span></span>  <br/> |
|<span data-ttu-id="b1cac-122">Installer</span><span class="sxs-lookup"><span data-stu-id="b1cac-122">Install</span></span>  <br/> |<span data-ttu-id="b1cac-123">Indique une action de l’installation.</span><span class="sxs-lookup"><span data-stu-id="b1cac-123">Indicates an installation action.</span></span>  <br/> |
|<span data-ttu-id="b1cac-124">Désinstaller</span><span class="sxs-lookup"><span data-stu-id="b1cac-124">Uninstall</span></span>  <br/> |<span data-ttu-id="b1cac-125">Indique une action de désinstallation.</span><span class="sxs-lookup"><span data-stu-id="b1cac-125">Indicates an uninstallation action.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b1cac-126">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b1cac-126">Child elements</span></span>

|<span data-ttu-id="b1cac-127">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b1cac-127">**Element**</span></span>|<span data-ttu-id="b1cac-128">**Description**</span><span class="sxs-lookup"><span data-stu-id="b1cac-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1cac-129">ClientExtension</span><span class="sxs-lookup"><span data-stu-id="b1cac-129">ClientExtension</span></span>](clientextension.md) <br/> |<span data-ttu-id="b1cac-130">Contient des informations utilisateur et de configuration relatives à une application.</span><span class="sxs-lookup"><span data-stu-id="b1cac-130">Contains user and configuration information about an app.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b1cac-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b1cac-131">Parent elements</span></span>

|<span data-ttu-id="b1cac-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b1cac-132">**Element**</span></span>|<span data-ttu-id="b1cac-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="b1cac-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1cac-134">Actions (ArrayOfSetClientExtensionActionsType)</span><span class="sxs-lookup"><span data-stu-id="b1cac-134">Actions (ArrayOfSetClientExtensionActionsType)</span></span>](actions-arrayofsetclientextensionactionstype.md) <br/> |<span data-ttu-id="b1cac-135">Spécifie un tableau des éléments **d’Action** .</span><span class="sxs-lookup"><span data-stu-id="b1cac-135">Specifies an array of **Action** elements.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b1cac-136">Remarques</span><span class="sxs-lookup"><span data-stu-id="b1cac-136">Remarks</span></span>

<span data-ttu-id="b1cac-137">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b1cac-137">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b1cac-138">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1cac-138">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1cac-139">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b1cac-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1cac-140">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b1cac-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b1cac-141">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b1cac-141">Schema Name</span></span>  <br/> |<span data-ttu-id="b1cac-142">Schéma type</span><span class="sxs-lookup"><span data-stu-id="b1cac-142">Type schema</span></span>  <br/> |
|<span data-ttu-id="b1cac-143">Validation File</span><span class="sxs-lookup"><span data-stu-id="b1cac-143">Validation File</span></span>  <br/> |<span data-ttu-id="b1cac-144">types.xsd</span><span class="sxs-lookup"><span data-stu-id="b1cac-144">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b1cac-145">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b1cac-145">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b1cac-146">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b1cac-146">See also</span></span>

- [<span data-ttu-id="b1cac-147">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b1cac-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

