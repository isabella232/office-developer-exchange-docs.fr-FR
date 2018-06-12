---
title: Ignorer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Ignore
api_type:
- schema
ms.assetid: 7789eec5-ceec-43f2-84d5-d0d15b734076
description: L’élément ignorer identifiant les éléments à ignorer lors de la synchronisation.
ms.openlocfilehash: 0ecff9bfeb1257552b7e52c0115e9e814edecd4b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827858"
---
# <a name="ignore"></a><span data-ttu-id="0f86e-103">Ignorer</span><span class="sxs-lookup"><span data-stu-id="0f86e-103">Ignore</span></span>

<span data-ttu-id="0f86e-104">L’élément **Ignorer** identifiant les éléments à ignorer lors de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="0f86e-104">The **Ignore** element identifies items to skip during synchronization.</span></span> 
  
[<span data-ttu-id="0f86e-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0f86e-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="0f86e-106">Ignorer</span><span class="sxs-lookup"><span data-stu-id="0f86e-106">Ignore</span></span>](ignore.md)
  
```xml
<Ignore>
   <ItemId/>
</Ignore>
```

 <span data-ttu-id="0f86e-107">**ArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="0f86e-107">**ArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0f86e-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="0f86e-108">Attributes and elements</span></span>

<span data-ttu-id="0f86e-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="0f86e-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0f86e-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="0f86e-110">Attributes</span></span>

<span data-ttu-id="0f86e-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="0f86e-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0f86e-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="0f86e-112">Child elements</span></span>

|<span data-ttu-id="0f86e-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f86e-113">**Element**</span></span>|<span data-ttu-id="0f86e-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f86e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f86e-115">ID d’élément</span><span class="sxs-lookup"><span data-stu-id="0f86e-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="0f86e-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f86e-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0f86e-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="0f86e-117">Parent elements</span></span>

|<span data-ttu-id="0f86e-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="0f86e-118">**Element**</span></span>|<span data-ttu-id="0f86e-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="0f86e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0f86e-120">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0f86e-120">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="0f86e-121">Définit une demande pour synchroniser des éléments dans un dossier de la banque Exchange.</span><span class="sxs-lookup"><span data-stu-id="0f86e-121">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0f86e-122">Note</span><span class="sxs-lookup"><span data-stu-id="0f86e-122">Remarks</span></span>

<span data-ttu-id="0f86e-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="0f86e-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0f86e-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="0f86e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0f86e-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="0f86e-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0f86e-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="0f86e-126">Schema name</span></span>  <br/> |<span data-ttu-id="0f86e-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="0f86e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0f86e-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="0f86e-128">Validation file</span></span>  <br/> |<span data-ttu-id="0f86e-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0f86e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0f86e-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="0f86e-130">Can be empty</span></span>  <br/> |<span data-ttu-id="0f86e-131">False</span><span class="sxs-lookup"><span data-stu-id="0f86e-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0f86e-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="0f86e-132">See also</span></span>



[<span data-ttu-id="0f86e-133">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="0f86e-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="0f86e-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="0f86e-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

