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
description: L’élément DelegateUsers contient les identités des délégués à ajouter à ou mettre à jour dans une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 69f5aab65634f41ec0f820da05dee79a300fb32e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457374"
---
# <a name="delegateusers"></a><span data-ttu-id="2d6b3-104">DelegateUsers</span><span class="sxs-lookup"><span data-stu-id="2d6b3-104">DelegateUsers</span></span>

<span data-ttu-id="2d6b3-105">L’élément **DelegateUsers** contient les identités des délégués à ajouter à ou mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d6b3-105">The **DelegateUsers** element contains the identities of delegates to add to or update in a mailbox.</span></span> <span data-ttu-id="2d6b3-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2d6b3-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DelegateUsers>
   <DelegateUser>
</DelegateUsers>
```

<span data-ttu-id="2d6b3-107">**ArrayOfDelegateUserType**</span><span class="sxs-lookup"><span data-stu-id="2d6b3-107">**ArrayOfDelegateUserType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2d6b3-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2d6b3-108">Attributes and elements</span></span>

<span data-ttu-id="2d6b3-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2d6b3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d6b3-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="2d6b3-110">Attributes</span></span>

<span data-ttu-id="2d6b3-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2d6b3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d6b3-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2d6b3-112">Child elements</span></span>

|<span data-ttu-id="2d6b3-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2d6b3-113">**Element**</span></span>|<span data-ttu-id="2d6b3-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2d6b3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d6b3-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="2d6b3-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="2d6b3-116">Identifie un seul délégué à ajouter à ou à mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d6b3-116">Identifies a single delegate to add to or update in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2d6b3-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2d6b3-117">Parent elements</span></span>

|<span data-ttu-id="2d6b3-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2d6b3-118">**Element**</span></span>|<span data-ttu-id="2d6b3-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="2d6b3-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d6b3-120">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="2d6b3-120">AddDelegate</span></span>](adddelegate.md) <br/> |<span data-ttu-id="2d6b3-121">Définit une demande d’ajout de délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d6b3-121">Defines a request to add delegates to a mailbox.</span></span> <span data-ttu-id="2d6b3-122">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2d6b3-122">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
|[<span data-ttu-id="2d6b3-123">UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="2d6b3-123">UpdateDelegate</span></span>](updatedelegate.md) <br/> |<span data-ttu-id="2d6b3-124">Définit une demande de mise à jour des délégués dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="2d6b3-124">Defines a request to update delegates in a mailbox.</span></span> <span data-ttu-id="2d6b3-125">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="2d6b3-125">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2d6b3-126">Remarques</span><span class="sxs-lookup"><span data-stu-id="2d6b3-126">Remarks</span></span>

<span data-ttu-id="2d6b3-127">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="2d6b3-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d6b3-128">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2d6b3-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d6b3-129">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2d6b3-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2d6b3-130">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2d6b3-130">Schema Name</span></span>  <br/> |<span data-ttu-id="2d6b3-131">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="2d6b3-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2d6b3-132">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2d6b3-132">Validation File</span></span>  <br/> |<span data-ttu-id="2d6b3-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="2d6b3-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2d6b3-134">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2d6b3-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d6b3-135">False</span><span class="sxs-lookup"><span data-stu-id="2d6b3-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d6b3-136">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2d6b3-136">See also</span></span>

- [<span data-ttu-id="2d6b3-137">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="2d6b3-137">AddDelegate operation</span></span>](adddelegate-operation.md) 
- [<span data-ttu-id="2d6b3-138">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="2d6b3-138">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="2d6b3-139">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2d6b3-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="2d6b3-140">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="2d6b3-140">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

