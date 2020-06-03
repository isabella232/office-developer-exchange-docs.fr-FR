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
description: L’élément RemoveDelegate définit une demande de suppression des délégués d’une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: eca357ad1ed2dc692f9f192b97abd3a5d765fafb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465519"
---
# <a name="removedelegate"></a><span data-ttu-id="817ff-104">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="817ff-104">RemoveDelegate</span></span>

<span data-ttu-id="817ff-105">L’élément **RemoveDelegate** définit une demande de suppression des délégués d’une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="817ff-105">The **RemoveDelegate** element defines a request to remove delegates from a mailbox.</span></span> <span data-ttu-id="817ff-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="817ff-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<RemoveDelegate>
      <Mailbox/>
   <UserIds/>
</RemoveDelegate>
```

 <span data-ttu-id="817ff-107">**RemoveDelegateType**</span><span class="sxs-lookup"><span data-stu-id="817ff-107">**RemoveDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="817ff-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="817ff-108">Attributes and elements</span></span>

<span data-ttu-id="817ff-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="817ff-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="817ff-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="817ff-110">Attributes</span></span>

<span data-ttu-id="817ff-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="817ff-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="817ff-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="817ff-112">Child elements</span></span>

|<span data-ttu-id="817ff-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="817ff-113">**Element**</span></span>|<span data-ttu-id="817ff-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="817ff-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="817ff-115">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="817ff-115">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="817ff-116">Identifie la boîte aux lettres du principal.</span><span class="sxs-lookup"><span data-stu-id="817ff-116">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="817ff-117">UserIds</span><span class="sxs-lookup"><span data-stu-id="817ff-117">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="817ff-118">Contient un tableau d’utilisateurs délégués à supprimer de la boîte aux lettres d’un principal.</span><span class="sxs-lookup"><span data-stu-id="817ff-118">Contains an array of delegate users to remove from a principal's mailbox.</span></span> <span data-ttu-id="817ff-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="817ff-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="817ff-120">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="817ff-120">Parent elements</span></span>

<span data-ttu-id="817ff-121">Aucun.</span><span class="sxs-lookup"><span data-stu-id="817ff-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="817ff-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="817ff-122">Remarks</span></span>

<span data-ttu-id="817ff-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="817ff-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="817ff-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="817ff-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="817ff-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="817ff-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="817ff-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="817ff-126">Schema Name</span></span>  <br/> |<span data-ttu-id="817ff-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="817ff-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="817ff-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="817ff-128">Validation File</span></span>  <br/> |<span data-ttu-id="817ff-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="817ff-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="817ff-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="817ff-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="817ff-131">False</span><span class="sxs-lookup"><span data-stu-id="817ff-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="817ff-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="817ff-132">See also</span></span>



[<span data-ttu-id="817ff-133">Opération RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="817ff-133">RemoveDelegate operation</span></span>](removedelegate-operation.md)


- [<span data-ttu-id="817ff-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="817ff-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

