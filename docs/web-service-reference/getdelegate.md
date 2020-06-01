---
title: GetDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegate
api_type:
- schema
ms.assetid: 6d5efe59-596f-46f8-bdc6-ca9cded9bb8e
description: L’élément GetDelegate définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: bd7fb55800b51eb2d69184bc4e04cdef3e6b9a89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461029"
---
# <a name="getdelegate"></a><span data-ttu-id="20a20-104">GetDelegate</span><span class="sxs-lookup"><span data-stu-id="20a20-104">GetDelegate</span></span>

<span data-ttu-id="20a20-105">L’élément **GetDelegate** définit une demande pour obtenir des informations sur les délégués à une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="20a20-105">The **GetDelegate** element defines a request to get information about delegates to a mailbox.</span></span> <span data-ttu-id="20a20-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="20a20-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<GetDelegate IncludePermissions="">
      <Mailbox/>
   <UserIds/>
</GetDelegate>
```

 <span data-ttu-id="20a20-107">**GetDelegateType**</span><span class="sxs-lookup"><span data-stu-id="20a20-107">**GetDelegateType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20a20-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="20a20-108">Attributes and elements</span></span>

<span data-ttu-id="20a20-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="20a20-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20a20-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="20a20-110">Attributes</span></span>

|<span data-ttu-id="20a20-111">**Attribut**</span><span class="sxs-lookup"><span data-stu-id="20a20-111">**Attribute**</span></span>|<span data-ttu-id="20a20-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="20a20-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="20a20-113">**IncludePermissions**</span><span class="sxs-lookup"><span data-stu-id="20a20-113">**IncludePermissions**</span></span> <br/> |<span data-ttu-id="20a20-114">Indique si la réponse contient des paramètres d’autorisation pour chaque utilisateur délégué.</span><span class="sxs-lookup"><span data-stu-id="20a20-114">Indicates whether the response contains permission settings for each delegate user.</span></span>  <br/> |
   
#### <a name="includepermissions-attribute-values"></a><span data-ttu-id="20a20-115">Valeurs d’attribut IncludePermissions</span><span class="sxs-lookup"><span data-stu-id="20a20-115">IncludePermissions attribute values</span></span>

|<span data-ttu-id="20a20-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="20a20-116">**Value**</span></span>|<span data-ttu-id="20a20-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="20a20-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="20a20-118">**True**</span><span class="sxs-lookup"><span data-stu-id="20a20-118">**True**</span></span> <br/> |<span data-ttu-id="20a20-119">Les autorisations des utilisateurs délégués sont renvoyées en plus des informations utilisateur des délégués qui sont renvoyées dans l’élément [userid](userid.md) .</span><span class="sxs-lookup"><span data-stu-id="20a20-119">Delegate user permissions are returned in addition to the delegate user information that is returned in the [UserId](userid.md) element.</span></span>  <br/> |
|<span data-ttu-id="20a20-120">**False**</span><span class="sxs-lookup"><span data-stu-id="20a20-120">**False**</span></span> <br/> |<span data-ttu-id="20a20-121">Les informations de l' [utilisateur](userid.md) sont renvoyées.</span><span class="sxs-lookup"><span data-stu-id="20a20-121">[UserId](userid.md) information is returned.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="20a20-122">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="20a20-122">Child elements</span></span>

|<span data-ttu-id="20a20-123">**Élément**</span><span class="sxs-lookup"><span data-stu-id="20a20-123">**Element**</span></span>|<span data-ttu-id="20a20-124">**Description**</span><span class="sxs-lookup"><span data-stu-id="20a20-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20a20-125">Boîte aux lettres</span><span class="sxs-lookup"><span data-stu-id="20a20-125">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="20a20-126">Identifie la boîte aux lettres du principal.</span><span class="sxs-lookup"><span data-stu-id="20a20-126">Identifies the principal's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="20a20-127">UserIds</span><span class="sxs-lookup"><span data-stu-id="20a20-127">UserIds</span></span>](userids.md) <br/> |<span data-ttu-id="20a20-128">Contient un tableau d’utilisateurs délégués à obtenir à partir de la boîte aux lettres d’un principal.</span><span class="sxs-lookup"><span data-stu-id="20a20-128">Contains an array of delegate users to get from a principal's mailbox.</span></span> <span data-ttu-id="20a20-129">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="20a20-129">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="20a20-130">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="20a20-130">Parent elements</span></span>

<span data-ttu-id="20a20-131">Aucun.</span><span class="sxs-lookup"><span data-stu-id="20a20-131">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="20a20-132">Remarques</span><span class="sxs-lookup"><span data-stu-id="20a20-132">Remarks</span></span>

<span data-ttu-id="20a20-133">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="20a20-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20a20-134">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="20a20-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20a20-135">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="20a20-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="20a20-136">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="20a20-136">Schema Name</span></span>  <br/> |<span data-ttu-id="20a20-137">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="20a20-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="20a20-138">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="20a20-138">Validation File</span></span>  <br/> |<span data-ttu-id="20a20-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="20a20-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20a20-140">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="20a20-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="20a20-141">False</span><span class="sxs-lookup"><span data-stu-id="20a20-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20a20-142">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20a20-142">See also</span></span>



[<span data-ttu-id="20a20-143">Opération GetDelegate</span><span class="sxs-lookup"><span data-stu-id="20a20-143">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="20a20-144">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="20a20-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

