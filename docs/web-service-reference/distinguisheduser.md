---
title: DistinguishedUser
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedUser
api_type:
- schema
ms.assetid: 9362699d-666a-4acf-8fa1-c6669f0a2ae5
description: L’élément DistinguishedUser identifie les comptes d’utilisateur anonymes et par défaut pour l’accès délégué. Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).
ms.openlocfilehash: 922c36251290d7090cdafbed9e570144593ca97e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530732"
---
# <a name="distinguisheduser"></a><span data-ttu-id="15207-104">DistinguishedUser</span><span class="sxs-lookup"><span data-stu-id="15207-104">DistinguishedUser</span></span>

<span data-ttu-id="15207-105">L’élément **DistinguishedUser** identifie les comptes d’utilisateur anonymes et par défaut pour l’accès délégué.</span><span class="sxs-lookup"><span data-stu-id="15207-105">The **DistinguishedUser** element identifies Anonymous and Default user accounts for delegate access.</span></span> <span data-ttu-id="15207-106">Cet élément a été introduit dans Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="15207-106">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span> 
  
```xml
<DistinguishedUser>Default or Anonymous</DistinguishedUser>
```

 <span data-ttu-id="15207-107">**DistinguishedUserType**</span><span class="sxs-lookup"><span data-stu-id="15207-107">**DistinguishedUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15207-108">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="15207-108">Attributes and elements</span></span>

<span data-ttu-id="15207-109">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="15207-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15207-110">Attributs</span><span class="sxs-lookup"><span data-stu-id="15207-110">Attributes</span></span>

<span data-ttu-id="15207-111">Aucune.</span><span class="sxs-lookup"><span data-stu-id="15207-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15207-112">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="15207-112">Child elements</span></span>

<span data-ttu-id="15207-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="15207-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15207-114">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="15207-114">Parent elements</span></span>

|<span data-ttu-id="15207-115">**Élément**</span><span class="sxs-lookup"><span data-stu-id="15207-115">**Element**</span></span>|<span data-ttu-id="15207-116">**Description**</span><span class="sxs-lookup"><span data-stu-id="15207-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15207-117">UserId</span><span class="sxs-lookup"><span data-stu-id="15207-117">UserId</span></span>](userid.md) <br/> |<span data-ttu-id="15207-118">Identifie un utilisateur délégué ou un utilisateur qui dispose des autorisations d’accès au dossier.</span><span class="sxs-lookup"><span data-stu-id="15207-118">Identifies a delegate user or a user who has folder access permissions.</span></span> <span data-ttu-id="15207-119">Cet élément a été introduit dans Exchange 2007 SP1.</span><span class="sxs-lookup"><span data-stu-id="15207-119">This element was introduced in Exchange 2007 SP1.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15207-120">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="15207-120">Text value</span></span>

<span data-ttu-id="15207-121">Une valeur de texte **par défaut** décrit le paramètre par défaut pour les utilisateurs délégués ajoutés à la boîte aux lettres du principal.</span><span class="sxs-lookup"><span data-stu-id="15207-121">A text value of **Default** describes the default setting for delegate users who are added to the principal's mailbox.</span></span> <span data-ttu-id="15207-122">Une valeur de texte **anonyme** décrit les paramètres d’accès délégué dont disposent les utilisateurs anonymes sur la boîte aux lettres de l’entité.</span><span class="sxs-lookup"><span data-stu-id="15207-122">A text value of **Anonymous** describes the delegate access settings that anonymous users have on the principal's mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="15207-123">Remarques</span><span class="sxs-lookup"><span data-stu-id="15207-123">Remarks</span></span>

<span data-ttu-id="15207-124">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute Microsoft Exchange Server 2007 sur lequel le rôle de serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="15207-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15207-125">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="15207-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15207-126">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="15207-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15207-127">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="15207-127">Schema Name</span></span>  <br/> |<span data-ttu-id="15207-128">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="15207-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="15207-129">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="15207-129">Validation File</span></span>  <br/> |<span data-ttu-id="15207-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="15207-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15207-131">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="15207-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="15207-132">False</span><span class="sxs-lookup"><span data-stu-id="15207-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15207-133">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="15207-133">See also</span></span>

- [<span data-ttu-id="15207-134">Opération AddDelegate</span><span class="sxs-lookup"><span data-stu-id="15207-134">AddDelegate operation</span></span>](adddelegate-operation.md)  
- [<span data-ttu-id="15207-135">Opération UpdateDelegate</span><span class="sxs-lookup"><span data-stu-id="15207-135">UpdateDelegate operation</span></span>](updatedelegate-operation.md)
- [<span data-ttu-id="15207-136">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15207-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="15207-137">Ajout de délégués</span><span class="sxs-lookup"><span data-stu-id="15207-137">Adding Delegates</span></span>](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

