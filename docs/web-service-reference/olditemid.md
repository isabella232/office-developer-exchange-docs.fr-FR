---
title: OldItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldItemId
api_type:
- schema
ms.assetid: fb57deee-9cc3-4730-9805-ff34f39e3ab7
description: L’élément OldItemId contient l’identificateur unique de l’élément qui a été copié ou déplacé.
ms.openlocfilehash: 9fab14478ffbb2dd8ad013d59520af943584f2eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467465"
---
# <a name="olditemid"></a><span data-ttu-id="b542e-103">OldItemId</span><span class="sxs-lookup"><span data-stu-id="b542e-103">OldItemId</span></span>

<span data-ttu-id="b542e-104">L’élément **OldItemId** contient l’identificateur unique de l’élément qui a été copié ou déplacé.</span><span class="sxs-lookup"><span data-stu-id="b542e-104">The **OldItemId** element contains the unique identifier of the item that was copied or moved.</span></span> 
  
```xml
<OldItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="b542e-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="b542e-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b542e-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b542e-106">Attributes and elements</span></span>

<span data-ttu-id="b542e-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b542e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b542e-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b542e-108">Attributes</span></span>

|<span data-ttu-id="b542e-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="b542e-109">**Attribute**</span></span>|<span data-ttu-id="b542e-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="b542e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b542e-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="b542e-111">**Id**</span></span> <br/> |<span data-ttu-id="b542e-112">Contient une chaîne qui identifie un élément dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="b542e-112">Contains a string that identifies an item in the Exchange store.</span></span> <span data-ttu-id="b542e-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="b542e-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="b542e-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="b542e-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="b542e-115">Contient une chaîne qui identifie une version d’un élément identifiée par l’attribut ID.</span><span class="sxs-lookup"><span data-stu-id="b542e-115">Contains a string that identifies a version of an item that is identified by the Id attribute.</span></span> <span data-ttu-id="b542e-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="b542e-116">This attribute is optional.</span></span> <span data-ttu-id="b542e-117">Utilisez cet attribut pour vous assurer que la version correcte d’un élément est utilisée.</span><span class="sxs-lookup"><span data-stu-id="b542e-117">Use this attribute to make sure that the correct version of an item is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b542e-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b542e-118">Child elements</span></span>

<span data-ttu-id="b542e-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b542e-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b542e-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b542e-120">Parent elements</span></span>

|<span data-ttu-id="b542e-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="b542e-121">**Element**</span></span>|<span data-ttu-id="b542e-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="b542e-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b542e-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="b542e-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="b542e-124">Représente un événement dans lequel un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="b542e-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="b542e-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="b542e-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="b542e-126">Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.</span><span class="sxs-lookup"><span data-stu-id="b542e-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b542e-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="b542e-127">Remarks</span></span>

<span data-ttu-id="b542e-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="b542e-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b542e-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b542e-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b542e-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b542e-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b542e-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b542e-131">Schema Name</span></span>  <br/> |<span data-ttu-id="b542e-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="b542e-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="b542e-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b542e-133">Validation File</span></span>  <br/> |<span data-ttu-id="b542e-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b542e-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b542e-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b542e-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="b542e-136">False</span><span class="sxs-lookup"><span data-stu-id="b542e-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b542e-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="b542e-137">See also</span></span>



[<span data-ttu-id="b542e-138">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="b542e-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="b542e-139">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="b542e-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="b542e-140">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="b542e-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="b542e-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="b542e-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

