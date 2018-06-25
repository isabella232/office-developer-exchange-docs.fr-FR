---
title: DelegateUsers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DelegateUsers
api_type:
- schema
ms.assetid: f30f80d9-20c8-41cc-afc7-a5eec1e0c5ea
description: L’élément DelegateUsers contient les identités de délégués à ajouter ou mettre à jour dans une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: a078707ae6b1676ca5a32ba718add93debd498fe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755836"
---
# <a name="delegateusers"></a><span data-ttu-id="a8743-104">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="a8743-104">DelegateUsers</span></span>

<span data-ttu-id="a8743-105">L’élément **DelegateUsers** contient les identités de délégués à ajouter ou mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a8743-105">The **DelegateUsers** element contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="a8743-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a8743-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUsers>
   <DelegateUser>
</DelegateUsers>
```

<span data-ttu-id="a8743-107">**ArrayOfDelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="a8743-107">**ArrayOfDelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a8743-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a8743-108">Attributes and elements</span></span>

<span data-ttu-id="a8743-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a8743-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8743-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="a8743-110">Attributes</span></span>

<span data-ttu-id="a8743-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="a8743-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8743-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a8743-112">Child elements</span></span>

|<span data-ttu-id="a8743-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8743-113">**Element**</span></span>|<span data-ttu-id="a8743-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8743-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8743-115">Utilisateur_délégué</span><span class="sxs-lookup"><span data-stu-id="a8743-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="a8743-116">Identifie un délégué unique à ajouter ou mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a8743-116">Identifies a single delegate to add to or update in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a8743-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a8743-117">Parent elements</span></span>

|<span data-ttu-id="a8743-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="a8743-118">**Element**</span></span>|<span data-ttu-id="a8743-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="a8743-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8743-120">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="a8743-120">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="a8743-121">Définit une demande pour ajouter des délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a8743-121">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="a8743-122">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a8743-122">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="a8743-123">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="a8743-123">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="a8743-124">Définit une demande de mise à jour des délégués dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="a8743-124">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="a8743-125">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a8743-125">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a8743-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="a8743-126">Remarks</span></span>

<span data-ttu-id="a8743-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="a8743-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8743-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a8743-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8743-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a8743-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a8743-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a8743-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a8743-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a8743-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a8743-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a8743-132">Validation File</span></span>  <br/> |<span data-ttu-id="a8743-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a8743-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a8743-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a8743-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8743-135">False</span><span class="sxs-lookup"><span data-stu-id="a8743-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8743-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="a8743-136">See also</span></span>

- [<span data-ttu-id="a8743-137">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="a8743-137">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="a8743-138">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="a8743-138">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="a8743-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="a8743-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="a8743-140">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="a8743-140">Adding Delegates</span></span>](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

