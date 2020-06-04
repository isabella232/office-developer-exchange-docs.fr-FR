---
title: ViewPrivateItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ViewPrivateItems
api_type:
- schema
ms.assetid: 80b949ac-440c-4a01-b428-ebafb5b1b802
description: L’élément ViewPrivateItems indique si un utilisateur délégué ou une application cliente a l’autorisation d’afficher des éléments privés dans la boîte aux lettres de l’entité de sécurité.
ms.openlocfilehash: 4e1375f7c4a3c660cc5de885deff8d094250ca7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44525968"
---
# <a name="viewprivateitems"></a><span data-ttu-id="d9cc8-103">ViewPrivateItems</span><span class="sxs-lookup"><span data-stu-id="d9cc8-103">ViewPrivateItems</span></span>

<span data-ttu-id="d9cc8-104">L’élément **ViewPrivateItems** indique si un utilisateur délégué ou une application cliente a l’autorisation d’afficher des éléments privés dans la boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="d9cc8-104">The **ViewPrivateItems** element indicates whether a delegate user or client application has permission to view private items in the principal's mailbox.</span></span> 
  
```XML
<ViewPrivateItems>true | false</ViewPrivateItems>
```

 <span data-ttu-id="d9cc8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d9cc8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9cc8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d9cc8-106">Attributes and elements</span></span>

<span data-ttu-id="d9cc8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d9cc8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9cc8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d9cc8-108">Attributes</span></span>

<span data-ttu-id="d9cc8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="d9cc8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d9cc8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d9cc8-110">Child elements</span></span>

<span data-ttu-id="d9cc8-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d9cc8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d9cc8-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d9cc8-112">Parent elements</span></span>

|<span data-ttu-id="d9cc8-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d9cc8-113">**Element**</span></span>|<span data-ttu-id="d9cc8-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d9cc8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9cc8-115">DelegateUser</span><span class="sxs-lookup"><span data-stu-id="d9cc8-115">DelegateUser</span></span>](delegateuser.md) <br/> |<span data-ttu-id="d9cc8-116">Identifie un seul délégué à ajouter ou mettre à jour dans une boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="d9cc8-116">Identifies a single delegate to add or update in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d9cc8-117">EffectiveRights</span><span class="sxs-lookup"><span data-stu-id="d9cc8-117">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="d9cc8-p101">Contient les droits du client en fonction des paramètres d'autorisation pour l'élément ou le dossier. Cet élément est en lecture seule.</span><span class="sxs-lookup"><span data-stu-id="d9cc8-p101">Contains the client's rights based on the permission settings for the item or folder. This element is read-only.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d9cc8-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="d9cc8-120">Text value</span></span>

<span data-ttu-id="d9cc8-121">La valeur **true** indique que le délégué ou le client peuvent afficher des éléments privés dans la boîte aux lettres de l’entité de sécurité.</span><span class="sxs-lookup"><span data-stu-id="d9cc8-121">A value of **true** indicates that the delegate or client can view private items in the principal's mailbox.</span></span> <span data-ttu-id="d9cc8-122">La valeur **false** indique que les éléments privés ne sont pas visibles par un délégué ou un client.</span><span class="sxs-lookup"><span data-stu-id="d9cc8-122">A value of **false** indicates that private items are not visible to a delegate or client.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d9cc8-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="d9cc8-123">Remarks</span></span>

<span data-ttu-id="d9cc8-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9cc8-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d9cc8-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d9cc8-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9cc8-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d9cc8-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9cc8-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d9cc8-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d9cc8-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d9cc8-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9cc8-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d9cc8-129">Validation File</span></span>  <br/> |<span data-ttu-id="d9cc8-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d9cc8-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9cc8-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d9cc8-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9cc8-132">False</span><span class="sxs-lookup"><span data-stu-id="d9cc8-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9cc8-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d9cc8-133">See also</span></span>



[<span data-ttu-id="d9cc8-134">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="d9cc8-134">AddDelegate operation</span></span>](adddelegate-operation.md)
  
[<span data-ttu-id="d9cc8-135">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="d9cc8-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)


- [<span data-ttu-id="d9cc8-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d9cc8-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d9cc8-137">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="d9cc8-137">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

