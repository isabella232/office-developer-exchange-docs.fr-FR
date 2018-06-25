---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: L’élément SyncScope indique si uniquement les éléments ou les éléments et les informations associées au dossier sont renvoyés dans une réponse de la synchronisation.
ms.openlocfilehash: 847c0244a8847364e29ea584b0c0b721f00d3064
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838666"
---
# <a name="syncscope"></a><span data-ttu-id="6df2c-103">SyncScope</span><span class="sxs-lookup"><span data-stu-id="6df2c-103">SyncScope</span></span>

<span data-ttu-id="6df2c-104">L’élément **SyncScope** indique si uniquement les éléments ou les éléments et les informations associées au dossier sont renvoyés dans une réponse de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="6df2c-104">The **SyncScope** element specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 <span data-ttu-id="6df2c-105">**SyncFolderItemsScopeType**</span><span class="sxs-lookup"><span data-stu-id="6df2c-105">**SyncFolderItemsScopeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6df2c-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="6df2c-106">Attributes and elements</span></span>

<span data-ttu-id="6df2c-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="6df2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6df2c-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="6df2c-108">Attributes</span></span>

<span data-ttu-id="6df2c-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6df2c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6df2c-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="6df2c-110">Child elements</span></span>

<span data-ttu-id="6df2c-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="6df2c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6df2c-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="6df2c-112">Parent elements</span></span>

|<span data-ttu-id="6df2c-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="6df2c-113">**Element**</span></span>|<span data-ttu-id="6df2c-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="6df2c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6df2c-115">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="6df2c-115">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="6df2c-116">L’élément qui définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="6df2c-116">The element that defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="6df2c-117">Vous trouverez ci-dessous l’expression XPath pour cet élément :</span><span class="sxs-lookup"><span data-stu-id="6df2c-117">The following is the XPath expression to this element:</span></span>  <br/> <span data-ttu-id="6df2c-118">/ SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="6df2c-118">/SyncFolderItems</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6df2c-119">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="6df2c-119">Text value</span></span>

<span data-ttu-id="6df2c-120">Le tableau suivant répertorie les valeurs possibles pour l’élément **SyncScope** .</span><span class="sxs-lookup"><span data-stu-id="6df2c-120">The following table lists the possible values for the **SyncScope** element.</span></span> 
  
<span data-ttu-id="6df2c-121">**Valeurs des éléments SyncScope**</span><span class="sxs-lookup"><span data-stu-id="6df2c-121">**SyncScope element values**</span></span>

|<span data-ttu-id="6df2c-122">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="6df2c-122">**Value**</span></span>|<span data-ttu-id="6df2c-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="6df2c-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6df2c-124">NormalItems</span><span class="sxs-lookup"><span data-stu-id="6df2c-124">NormalItems</span></span>  <br/> |<span data-ttu-id="6df2c-125">Spécifie que seuls les éléments dans le dossier sont retournés dans une réponse de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="6df2c-125">Specifies that only items in the folder are returned in a synchronization response.</span></span>  <br/> |
|<span data-ttu-id="6df2c-126">NormalAndAssociatedItems</span><span class="sxs-lookup"><span data-stu-id="6df2c-126">NormalAndAssociatedItems</span></span>  <br/> |<span data-ttu-id="6df2c-127">Spécifie que les deux éléments dans le dossier et les informations associées au dossier sont retournés dans une réponse de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="6df2c-127">Specifies that both items in the folder and folder associated information are returned in a synchronization response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6df2c-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="6df2c-128">Remarks</span></span>

<span data-ttu-id="6df2c-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="6df2c-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6df2c-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="6df2c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6df2c-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="6df2c-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6df2c-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="6df2c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="6df2c-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="6df2c-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6df2c-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="6df2c-134">Validation File</span></span>  <br/> |<span data-ttu-id="6df2c-135">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6df2c-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6df2c-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="6df2c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="6df2c-137">False</span><span class="sxs-lookup"><span data-stu-id="6df2c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6df2c-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="6df2c-138">See also</span></span>



[<span data-ttu-id="6df2c-139">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="6df2c-139">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="6df2c-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="6df2c-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

