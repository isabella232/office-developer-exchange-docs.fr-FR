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
description: L’élément ignore identifie les éléments à ignorer lors de la synchronisation.
ms.openlocfilehash: b65d11d8c7655279dac0e7d3cbd13f8a9317540c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458571"
---
# <a name="ignore"></a><span data-ttu-id="5ab01-103">Ignorer</span><span class="sxs-lookup"><span data-stu-id="5ab01-103">Ignore</span></span>

<span data-ttu-id="5ab01-104">L’élément **ignore** identifie les éléments à ignorer lors de la synchronisation.</span><span class="sxs-lookup"><span data-stu-id="5ab01-104">The **Ignore** element identifies items to skip during synchronization.</span></span> 
  
[<span data-ttu-id="5ab01-105">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5ab01-105">SyncFolderItems</span></span>](syncfolderitems.md)
  
[<span data-ttu-id="5ab01-106">Ignore</span><span class="sxs-lookup"><span data-stu-id="5ab01-106">Ignore</span></span>](ignore.md)
  
```xml
<Ignore>
   <ItemId/>
</Ignore>
```

 <span data-ttu-id="5ab01-107">**ArrayOfBaseItemIdsType**</span><span class="sxs-lookup"><span data-stu-id="5ab01-107">**ArrayOfBaseItemIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ab01-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="5ab01-108">Attributes and elements</span></span>

<span data-ttu-id="5ab01-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="5ab01-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ab01-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="5ab01-110">Attributes</span></span>

<span data-ttu-id="5ab01-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="5ab01-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5ab01-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="5ab01-112">Child elements</span></span>

|<span data-ttu-id="5ab01-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ab01-113">**Element**</span></span>|<span data-ttu-id="5ab01-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ab01-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ab01-115">ItemId</span><span class="sxs-lookup"><span data-stu-id="5ab01-115">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="5ab01-116">Contient l'identificateur unique et la clé de modification d'un élément dans la banque d'informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ab01-116">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ab01-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="5ab01-117">Parent elements</span></span>

|<span data-ttu-id="5ab01-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="5ab01-118">**Element**</span></span>|<span data-ttu-id="5ab01-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="5ab01-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ab01-120">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5ab01-120">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="5ab01-121">Définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ab01-121">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5ab01-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="5ab01-122">Remarks</span></span>

<span data-ttu-id="5ab01-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="5ab01-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ab01-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="5ab01-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ab01-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="5ab01-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5ab01-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="5ab01-126">Schema name</span></span>  <br/> |<span data-ttu-id="5ab01-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="5ab01-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5ab01-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="5ab01-128">Validation file</span></span>  <br/> |<span data-ttu-id="5ab01-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="5ab01-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5ab01-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="5ab01-130">Can be empty</span></span>  <br/> |<span data-ttu-id="5ab01-131">False</span><span class="sxs-lookup"><span data-stu-id="5ab01-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ab01-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="5ab01-132">See also</span></span>



[<span data-ttu-id="5ab01-133">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="5ab01-133">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="5ab01-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="5ab01-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

