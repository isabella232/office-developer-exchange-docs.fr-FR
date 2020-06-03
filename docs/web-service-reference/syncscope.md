---
title: SyncScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncScope
api_type:
- schema
ms.assetid: e0ca231f-0374-4844-8d4c-ada8da167920
description: L’élément SyncScope spécifie si les éléments ou les éléments et les informations associés uniquement sont renvoyés dans une réponse de synchronisation.
ms.openlocfilehash: 5ede26204c823a452189222075c784f24e98d188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463033"
---
# <a name="syncscope"></a><span data-ttu-id="72508-103">SyncScope</span><span class="sxs-lookup"><span data-stu-id="72508-103">SyncScope</span></span>

<span data-ttu-id="72508-104">L’élément **SyncScope** spécifie si les éléments ou les éléments et les informations associés uniquement sont renvoyés dans une réponse de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="72508-104">The **SyncScope** element specifies whether just items or items and folder associated information are returned in a synchronization response.</span></span> 
  
```xml
<SyncScope>NormalItems or NormalAndAssociatedItems</SyncScope>
```

 <span data-ttu-id="72508-105">**SyncFolderItemsScopeType**</span><span class="sxs-lookup"><span data-stu-id="72508-105">**SyncFolderItemsScopeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72508-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="72508-106">Attributes and elements</span></span>

<span data-ttu-id="72508-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="72508-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72508-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="72508-108">Attributes</span></span>

<span data-ttu-id="72508-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="72508-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72508-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="72508-110">Child elements</span></span>

<span data-ttu-id="72508-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="72508-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72508-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="72508-112">Parent elements</span></span>

|<span data-ttu-id="72508-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="72508-113">**Element**</span></span>|<span data-ttu-id="72508-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="72508-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72508-115">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="72508-115">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="72508-116">Élément qui définit une demande de synchronisation des éléments dans un dossier de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="72508-116">The element that defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="72508-117">Voici l’expression XPath de cet élément :</span><span class="sxs-lookup"><span data-stu-id="72508-117">The following is the XPath expression to this element:</span></span>  <br/> <span data-ttu-id="72508-118">/SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="72508-118">/SyncFolderItems</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="72508-119">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="72508-119">Text value</span></span>

<span data-ttu-id="72508-120">Le tableau suivant répertorie les valeurs possibles pour l’élément **SyncScope** .</span><span class="sxs-lookup"><span data-stu-id="72508-120">The following table lists the possible values for the **SyncScope** element.</span></span> 
  
<span data-ttu-id="72508-121">**Valeurs de l’élément SyncScope**</span><span class="sxs-lookup"><span data-stu-id="72508-121">**SyncScope element values**</span></span>

|<span data-ttu-id="72508-122">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="72508-122">**Value**</span></span>|<span data-ttu-id="72508-123">**Description**</span><span class="sxs-lookup"><span data-stu-id="72508-123">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="72508-124">NormalItems</span><span class="sxs-lookup"><span data-stu-id="72508-124">NormalItems</span></span>  <br/> |<span data-ttu-id="72508-125">Spécifie que seuls les éléments du dossier sont renvoyés dans une réponse de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="72508-125">Specifies that only items in the folder are returned in a synchronization response.</span></span>  <br/> |
|<span data-ttu-id="72508-126">NormalAndAssociatedItems</span><span class="sxs-lookup"><span data-stu-id="72508-126">NormalAndAssociatedItems</span></span>  <br/> |<span data-ttu-id="72508-127">Spécifie que les deux éléments dans les informations associées au dossier et au dossier sont renvoyés dans une réponse de synchronisation.</span><span class="sxs-lookup"><span data-stu-id="72508-127">Specifies that both items in the folder and folder associated information are returned in a synchronization response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="72508-128">Remarques</span><span class="sxs-lookup"><span data-stu-id="72508-128">Remarks</span></span>

<span data-ttu-id="72508-129">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="72508-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72508-130">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="72508-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72508-131">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="72508-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="72508-132">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="72508-132">Schema Name</span></span>  <br/> |<span data-ttu-id="72508-133">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="72508-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="72508-134">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="72508-134">Validation File</span></span>  <br/> |<span data-ttu-id="72508-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="72508-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="72508-136">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="72508-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="72508-137">False</span><span class="sxs-lookup"><span data-stu-id="72508-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72508-138">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="72508-138">See also</span></span>



[<span data-ttu-id="72508-139">Opération SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="72508-139">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="72508-140">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="72508-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

