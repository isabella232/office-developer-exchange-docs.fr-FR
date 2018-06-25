---
title: RemoveDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegate
api_type:
- schema
ms.assetid: f21c5171-62e7-47c8-99b1-22e1ff5883bb
description: L’élément RemoveDelegate définit une demande pour supprimer des délégués d’une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 27618b1767c99b26a5f4c06e97a20e063b598d9d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829085"
---
# <a name="removedelegate"></a><span data-ttu-id="ffc69-104">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="ffc69-104">RemoveDelegate</span></span>

<span data-ttu-id="ffc69-105">L’élément **RemoveDelegate** définit une demande pour supprimer des délégués d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ffc69-105">The **RemoveDelegate** element defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="ffc69-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ffc69-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<RemoveDelegate>
      <Mailbox/>
   <UserIds/>
</RemoveDelegate>
```

 <span data-ttu-id="ffc69-107">**RemoveDelegateType**</span><span class="sxs-lookup"><span data-stu-id="ffc69-107">**RemoveDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ffc69-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ffc69-108">Attributes and elements</span></span>

<span data-ttu-id="ffc69-109">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ffc69-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ffc69-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="ffc69-110">Attributes</span></span>

<span data-ttu-id="ffc69-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ffc69-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ffc69-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ffc69-112">Child elements</span></span>

|<span data-ttu-id="ffc69-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ffc69-113">**Element**</span></span>|<span data-ttu-id="ffc69-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ffc69-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ffc69-115">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="ffc69-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="ffc69-116">Identifie la boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="ffc69-116">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ffc69-117">ID utilisateur</span><span class="sxs-lookup"><span data-stu-id="ffc69-117">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="ffc69-118">Contient un tableau d’utilisateurs délégué à supprimer de la boîte aux lettres d’un utilisateur principal.</span><span class="sxs-lookup"><span data-stu-id="ffc69-118">Contains an array of delegate users to remove from a principal's mailbox.</span></span> <span data-ttu-id="ffc69-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="ffc69-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ffc69-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ffc69-120">Parent elements</span></span>

<span data-ttu-id="ffc69-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ffc69-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ffc69-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="ffc69-122">Remarks</span></span>

<span data-ttu-id="ffc69-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ffc69-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ffc69-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ffc69-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ffc69-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ffc69-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ffc69-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ffc69-126">Schema Name</span></span>  <br/> |<span data-ttu-id="ffc69-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="ffc69-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ffc69-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ffc69-128">Validation File</span></span>  <br/> |<span data-ttu-id="ffc69-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="ffc69-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ffc69-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ffc69-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="ffc69-131">False</span><span class="sxs-lookup"><span data-stu-id="ffc69-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ffc69-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ffc69-132">See also</span></span>



[<span data-ttu-id="ffc69-133">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="ffc69-133">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="ffc69-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ffc69-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

