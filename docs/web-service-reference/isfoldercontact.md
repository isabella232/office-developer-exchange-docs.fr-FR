---
title: IsFolderContact
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsFolderContact
api_type:
- schema
ms.assetid: 8b456255-f4ae-4ca0-845a-13c195f1c867
description: L'élément IsFolderContact indique si un utilisateur est un contact d'un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: b7830a94237b721d02409e2d93b27c2c5ef015e7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455281"
---
# <a name="isfoldercontact"></a><span data-ttu-id="442ce-104">IsFolderContact</span><span class="sxs-lookup"><span data-stu-id="442ce-104">IsFolderContact</span></span>

<span data-ttu-id="442ce-p102">Ce document peut contenir des informations liées aux fonctionnalités ou produits préliminaires qui sont sujettes à modifications avant la sortie de la version définitive. Ce document est fourni "tel quel" à titre indicatif et Microsoft exclut toute garantie, expresse ou implicite, en ce qui concerne ce document. L'élément **IsFolderContact** indique si un utilisateur est un contact d'un dossier. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="442ce-p102">The **IsFolderContact** element indicates whether a user is a contact for a folder. This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<IsFolderContact/>
```

 <span data-ttu-id="442ce-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="442ce-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="442ce-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="442ce-108">Attributes and elements</span></span>

<span data-ttu-id="442ce-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="442ce-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="442ce-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="442ce-110">Attributes</span></span>

<span data-ttu-id="442ce-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="442ce-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="442ce-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="442ce-112">Child elements</span></span>

<span data-ttu-id="442ce-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="442ce-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="442ce-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="442ce-114">Parent elements</span></span>

|<span data-ttu-id="442ce-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="442ce-115">**Element**</span></span>|<span data-ttu-id="442ce-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="442ce-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="442ce-117">Autorisation</span><span class="sxs-lookup"><span data-stu-id="442ce-117">Permission</span></span>](permission.md) <br/> |<span data-ttu-id="442ce-p103">Définit l'accès dont dispose un utilisateur dans un dossier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="442ce-p103">Defines the access that a user has to a folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
|[<span data-ttu-id="442ce-120">CalendarPermission</span><span class="sxs-lookup"><span data-stu-id="442ce-120">CalendarPermission</span></span>](calendarpermission.md) <br/> |<span data-ttu-id="442ce-p104">Définit l'accès dont dispose un utilisateur dans un dossier de calendrier. Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="442ce-p104">Defines the access that a user has to a Calendar folder. This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="442ce-123">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="442ce-123">Text value</span></span>

<span data-ttu-id="442ce-p105">Une valeur texte **true** indique que l'utilisateur est un contact pour le dossier spécifié. La valeur **false** indique que l'utilisateur n'est pas un contact pour le dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="442ce-p105">A text value of **true** indicates that the user is a contact for the specified folder. A value of **false** indicates that the user is not a contact for the specified folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="442ce-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="442ce-126">Remarks</span></span>

<span data-ttu-id="442ce-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="442ce-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="442ce-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="442ce-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="442ce-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="442ce-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="442ce-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="442ce-130">Schema Name</span></span>  <br/> |<span data-ttu-id="442ce-131">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="442ce-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="442ce-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="442ce-132">Validation File</span></span>  <br/> |<span data-ttu-id="442ce-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="442ce-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="442ce-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="442ce-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="442ce-135">False</span><span class="sxs-lookup"><span data-stu-id="442ce-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="442ce-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="442ce-136">See also</span></span>



- [<span data-ttu-id="442ce-137">Éléments XML EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="442ce-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="442ce-138">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="442ce-138">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

