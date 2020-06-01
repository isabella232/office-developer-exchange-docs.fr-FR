---
title: OldFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldFolderId
api_type:
- schema
ms.assetid: da554a97-ab87-4950-9fc4-26b1972381bb
description: L’élément OldFolderId contient l’identificateur d’origine d’un dossier déplacé ou copié.
ms.openlocfilehash: a6713b9e0c47d68480724c3902086da6a8647dd7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458060"
---
# <a name="oldfolderid"></a><span data-ttu-id="88e1b-103">OldFolderId</span><span class="sxs-lookup"><span data-stu-id="88e1b-103">OldFolderId</span></span>

<span data-ttu-id="88e1b-104">L’élément **OldFolderId** contient l’identificateur d’origine d’un dossier déplacé ou copié.</span><span class="sxs-lookup"><span data-stu-id="88e1b-104">The **OldFolderId** element contains the original identifier of a folder that was moved or copied.</span></span> 
  
```xml
<OldFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="88e1b-105">**FolderIdType**</span><span class="sxs-lookup"><span data-stu-id="88e1b-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88e1b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="88e1b-106">Attributes and elements</span></span>

<span data-ttu-id="88e1b-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="88e1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88e1b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="88e1b-108">Attributes</span></span>

|<span data-ttu-id="88e1b-109">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="88e1b-109">**Attribute**</span></span>|<span data-ttu-id="88e1b-110">**Description**</span><span class="sxs-lookup"><span data-stu-id="88e1b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88e1b-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="88e1b-111">**Id**</span></span> <br/> |<span data-ttu-id="88e1b-112">Contient une chaîne qui identifie un dossier dans la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="88e1b-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="88e1b-113">Cet attribut est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="88e1b-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="88e1b-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="88e1b-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="88e1b-115">Contient une chaîne qui identifie la version d’un dossier identifiée par l’attribut ID.</span><span class="sxs-lookup"><span data-stu-id="88e1b-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="88e1b-116">Cet attribut est facultatif.</span><span class="sxs-lookup"><span data-stu-id="88e1b-116">This attribute is optional.</span></span> <span data-ttu-id="88e1b-117">Utilisez cet attribut pour vous assurer que la version correcte d’un dossier est utilisée.</span><span class="sxs-lookup"><span data-stu-id="88e1b-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="88e1b-118">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="88e1b-118">Child elements</span></span>

<span data-ttu-id="88e1b-119">Aucun.</span><span class="sxs-lookup"><span data-stu-id="88e1b-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="88e1b-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="88e1b-120">Parent elements</span></span>

|<span data-ttu-id="88e1b-121">**Élément**</span><span class="sxs-lookup"><span data-stu-id="88e1b-121">**Element**</span></span>|<span data-ttu-id="88e1b-122">**Description**</span><span class="sxs-lookup"><span data-stu-id="88e1b-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88e1b-123">CopiedEvent</span><span class="sxs-lookup"><span data-stu-id="88e1b-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="88e1b-124">Représente un événement dans lequel un élément ou un dossier est copié.</span><span class="sxs-lookup"><span data-stu-id="88e1b-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="88e1b-125">MovedEvent</span><span class="sxs-lookup"><span data-stu-id="88e1b-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="88e1b-126">Représente un événement dans lequel un élément ou un dossier est déplacé d’un dossier parent vers un autre dossier parent.</span><span class="sxs-lookup"><span data-stu-id="88e1b-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="88e1b-127">Remarques</span><span class="sxs-lookup"><span data-stu-id="88e1b-127">Remarks</span></span>

<span data-ttu-id="88e1b-128">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="88e1b-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88e1b-129">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="88e1b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88e1b-130">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="88e1b-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="88e1b-131">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="88e1b-131">Schema Name</span></span>  <br/> |<span data-ttu-id="88e1b-132">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="88e1b-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="88e1b-133">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="88e1b-133">Validation File</span></span>  <br/> |<span data-ttu-id="88e1b-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="88e1b-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="88e1b-135">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="88e1b-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="88e1b-136">False</span><span class="sxs-lookup"><span data-stu-id="88e1b-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88e1b-137">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="88e1b-137">See also</span></span>



[<span data-ttu-id="88e1b-138">Opération d'abonnement</span><span class="sxs-lookup"><span data-stu-id="88e1b-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="88e1b-139">Opération de GetEvents</span><span class="sxs-lookup"><span data-stu-id="88e1b-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="88e1b-140">Opération de résiliation d'abonnement</span><span class="sxs-lookup"><span data-stu-id="88e1b-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="88e1b-141">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="88e1b-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

