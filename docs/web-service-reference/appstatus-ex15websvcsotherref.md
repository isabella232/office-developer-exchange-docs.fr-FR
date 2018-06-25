---
title: AppStatus
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f3ab8bf1-abc5-45cf-a2e1-d7602f2c24ec
description: La valeur de l’élément AppStatus indique l’état de l’application de messagerie.
ms.openlocfilehash: cf213fc3d7be02c411e9c2e83a4ff153dbefe098
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755311"
---
# <a name="appstatus"></a><span data-ttu-id="e3539-103">AppStatus</span><span class="sxs-lookup"><span data-stu-id="e3539-103">AppStatus</span></span>

<span data-ttu-id="e3539-104">La valeur de l’élément **AppStatus** indique l’état de l’application de messagerie.</span><span class="sxs-lookup"><span data-stu-id="e3539-104">The **AppStatus** element value indicates the status of the mail app.</span></span> 
  
```XML
<AppStatus/>
```

 <span data-ttu-id="e3539-105">**string**</span><span class="sxs-lookup"><span data-stu-id="e3539-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3539-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="e3539-106">Attributes and elements</span></span>

<span data-ttu-id="e3539-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="e3539-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3539-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="e3539-108">Attributes</span></span>

<span data-ttu-id="e3539-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e3539-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3539-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="e3539-110">Child elements</span></span>

<span data-ttu-id="e3539-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="e3539-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e3539-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="e3539-112">Parent elements</span></span>

[<span data-ttu-id="e3539-113">Métadonnées</span><span class="sxs-lookup"><span data-stu-id="e3539-113">Metadata</span></span>](metadata-ex15websvcsotherref.md)
  
## <a name="text-value"></a><span data-ttu-id="e3539-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="e3539-114">Text value</span></span>

<span data-ttu-id="e3539-115">La valeur de texte de l’élément **AppStatus** indique l’état de l’application de messagerie.</span><span class="sxs-lookup"><span data-stu-id="e3539-115">The text value of the **AppStatus** element indicates the status of the mail app.</span></span> <span data-ttu-id="e3539-116">Si l’utilisateur peut résoudre un problème lié à l’état de l’application de messagerie, l’élément [ActionUrl](actionurl.md) fournit l’URL pour effectuer le correctif.</span><span class="sxs-lookup"><span data-stu-id="e3539-116">If the user can fix an issue related to the status of the mail app, the [ActionUrl](actionurl.md) element provides the URL to perform the fix.</span></span> 
  
<span data-ttu-id="e3539-117">**Le tableau 1. Valeurs AppStatus**</span><span class="sxs-lookup"><span data-stu-id="e3539-117">**Table 1. AppStatus values**</span></span>

|<span data-ttu-id="e3539-118">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="e3539-118">**Value**</span></span>|<span data-ttu-id="e3539-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="e3539-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e3539-120">NULL ou 0</span><span class="sxs-lookup"><span data-stu-id="e3539-120">Null or 0</span></span>  <br/> |<span data-ttu-id="e3539-121">L’application de messagerie a un état sain.</span><span class="sxs-lookup"><span data-stu-id="e3539-121">The mail app has a healthy status.</span></span>  <br/> |
|<span data-ttu-id="e3539-122">1.0</span><span class="sxs-lookup"><span data-stu-id="e3539-122">1.0</span></span>  <br/> |<span data-ttu-id="e3539-123">L’application de messagerie n’a pas pu être chargée automatiquement.</span><span class="sxs-lookup"><span data-stu-id="e3539-123">The mail app could not be automatically updated.</span></span> <span data-ttu-id="e3539-124">L’application de messagerie doit être installée à partir de l’Office Store.</span><span class="sxs-lookup"><span data-stu-id="e3539-124">The mail app needs to be re-installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="e3539-125">1.1</span><span class="sxs-lookup"><span data-stu-id="e3539-125">1.1</span></span>  <br/> |<span data-ttu-id="e3539-126">L’application de messagerie n’a pas pu être chargée automatiquement.</span><span class="sxs-lookup"><span data-stu-id="e3539-126">The mail app could not be automatically updated.</span></span> <span data-ttu-id="e3539-127">L’application de messagerie nécessite des autorisations accrues, mais ceci nécessite votre révision et confirmer l’installation.</span><span class="sxs-lookup"><span data-stu-id="e3539-127">The mail app requires increased permissions, and this requires your review and confirmation to install.</span></span>  <br/> |
|<span data-ttu-id="e3539-128">1.2</span><span class="sxs-lookup"><span data-stu-id="e3539-128">1.2</span></span>  <br/> |<span data-ttu-id="e3539-129">L’application de messagerie n’a pas pu être mis à jour automatiquement.</span><span class="sxs-lookup"><span data-stu-id="e3539-129">The mail app couldn't be updated automatically.</span></span> <span data-ttu-id="e3539-130">La licence actuelle a expiré ou n’est pas valide.</span><span class="sxs-lookup"><span data-stu-id="e3539-130">The current license has expired or is invalid.</span></span> <span data-ttu-id="e3539-131">Mettez à jour l’application de messagerie de l’Office Store.</span><span class="sxs-lookup"><span data-stu-id="e3539-131">Please update the mail app from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="e3539-132">2.0</span><span class="sxs-lookup"><span data-stu-id="e3539-132">2.0</span></span>  <br/> |<span data-ttu-id="e3539-133">La licence d’application de messagerie n’a pas pu être chargée automatiquement.</span><span class="sxs-lookup"><span data-stu-id="e3539-133">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="e3539-134">La licence pour l’application de messagerie doit être récupéré à partir de l’Office Store.</span><span class="sxs-lookup"><span data-stu-id="e3539-134">The license for the mail app needs to be recovered from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="e3539-135">2.1</span><span class="sxs-lookup"><span data-stu-id="e3539-135">2.1</span></span>  <br/> |<span data-ttu-id="e3539-136">La licence d’application de messagerie n’a pas pu être chargée automatiquement.</span><span class="sxs-lookup"><span data-stu-id="e3539-136">The mail app license could not be automatically updated.</span></span> <span data-ttu-id="e3539-137">La licence actuelle a expiré.</span><span class="sxs-lookup"><span data-stu-id="e3539-137">The current license has expired.</span></span> <span data-ttu-id="e3539-138">Une nouvelle licence pour cette application doit être installé à partir de l’Office Store.</span><span class="sxs-lookup"><span data-stu-id="e3539-138">A new license for this app needs to be installed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="e3539-139">3.0</span><span class="sxs-lookup"><span data-stu-id="e3539-139">3.0</span></span>  <br/> |<span data-ttu-id="e3539-140">L’état de l’Office Store pour l’application de messagerie a changé.</span><span class="sxs-lookup"><span data-stu-id="e3539-140">The Office Store status for the mail app has changed.</span></span> <span data-ttu-id="e3539-141">Cela peut indiquer qu’il existe un problème avec l’application de messagerie.</span><span class="sxs-lookup"><span data-stu-id="e3539-141">This may indicate that there is a problem with the mail app.</span></span> <span data-ttu-id="e3539-142">Accédez à la page d’application de messagerie dans l’Office Store pour plus d’informations.</span><span class="sxs-lookup"><span data-stu-id="e3539-142">Go to the mail app page in the Office Store for more information.</span></span>  <br/> |
|<span data-ttu-id="e3539-143">3.1</span><span class="sxs-lookup"><span data-stu-id="e3539-143">3.1</span></span>  <br/> |<span data-ttu-id="e3539-144">L’application de messagerie a été supprimée de l’Office Store.</span><span class="sxs-lookup"><span data-stu-id="e3539-144">The mail app has been removed from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="e3539-145">3.2</span><span class="sxs-lookup"><span data-stu-id="e3539-145">3.2</span></span>  <br/> |<span data-ttu-id="e3539-146">Un problème a été détecté avec l’application de messagerie et il a été temporairement retiré de l’Office Store.</span><span class="sxs-lookup"><span data-stu-id="e3539-146">A problem has been discovered with the mail app and it has temporarily been withdrawn from the Office Store.</span></span>  <br/> |
|<span data-ttu-id="e3539-147">3.3</span><span class="sxs-lookup"><span data-stu-id="e3539-147">3.3</span></span>  <br/> |<span data-ttu-id="e3539-148">L’application de messagerie sera supprimée du magasin de bureau dans les 30 jours.</span><span class="sxs-lookup"><span data-stu-id="e3539-148">The mail app will be removed from the Office Store within 30 days.</span></span>  <br/> |
|<span data-ttu-id="e3539-149">4.0</span><span class="sxs-lookup"><span data-stu-id="e3539-149">4.0</span></span>  <br/> |<span data-ttu-id="e3539-150">L’application de messagerie a été désactivée automatiquement par votre client de messagerie.</span><span class="sxs-lookup"><span data-stu-id="e3539-150">The mail app has been automatically disabled by your mail client.</span></span>  <br/> |
|<span data-ttu-id="e3539-151">4.1</span><span class="sxs-lookup"><span data-stu-id="e3539-151">4.1</span></span>  <br/> |<span data-ttu-id="e3539-152">L’application de messagerie a été désactivée par Outlook pour des raisons de performances.</span><span class="sxs-lookup"><span data-stu-id="e3539-152">The mail app has been disabled by Outlook for performance reasons.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3539-153">Remarques</span><span class="sxs-lookup"><span data-stu-id="e3539-153">Remarks</span></span>

<span data-ttu-id="e3539-154">Cet élément est une nouveauté d'Exchange Server 2013 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="e3539-154">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="e3539-155">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="e3539-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3539-156">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="e3539-156">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3539-157">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="e3539-157">Namespace</span></span>  <br/> | http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3539-158">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="e3539-158">Schema Name</span></span>  <br/> |<span data-ttu-id="e3539-159">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="e3539-159">Types schema</span></span>  <br/> |
|<span data-ttu-id="e3539-160">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="e3539-160">Validation File</span></span>  <br/> |<span data-ttu-id="e3539-161">Not applicable</span><span class="sxs-lookup"><span data-stu-id="e3539-161">Not applicable</span></span>  <br/> |
|<span data-ttu-id="e3539-162">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="e3539-162">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3539-163">False</span><span class="sxs-lookup"><span data-stu-id="e3539-163">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3539-164">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e3539-164">See also</span></span>

- [<span data-ttu-id="e3539-165">Métadonnées</span><span class="sxs-lookup"><span data-stu-id="e3539-165">Metadata</span></span>](metadata-ex15websvcsotherref.md)
- [<span data-ttu-id="e3539-166">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="e3539-166">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

