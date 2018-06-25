---
title: CanDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CanDelete
api_type:
- schema
ms.assetid: 55e17121-aad0-4f90-889f-2c3512e9579c
description: L’élément CanDelete indique si un dossier géré peut être supprimé par un client.
ms.openlocfilehash: b70b28bd6b3c9452f5d7f249f453218d555754da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755491"
---
# <a name="candelete"></a><span data-ttu-id="419e7-103">CanDelete</span><span class="sxs-lookup"><span data-stu-id="419e7-103">CanDelete</span></span>

<span data-ttu-id="419e7-104">L’élément **CanDelete** indique si un dossier géré peut être supprimé par un client.</span><span class="sxs-lookup"><span data-stu-id="419e7-104">The **CanDelete** element indicates whether a managed folder can be deleted by a customer.</span></span> 
  
```xml
<CanDelete/>
```

 <span data-ttu-id="419e7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="419e7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="419e7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="419e7-106">Attributes and elements</span></span>

<span data-ttu-id="419e7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="419e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="419e7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="419e7-108">Attributes</span></span>

<span data-ttu-id="419e7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="419e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="419e7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="419e7-110">Child elements</span></span>

<span data-ttu-id="419e7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="419e7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="419e7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="419e7-112">Parent elements</span></span>

|<span data-ttu-id="419e7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="419e7-113">**Element**</span></span>|<span data-ttu-id="419e7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="419e7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="419e7-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="419e7-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="419e7-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="419e7-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="419e7-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="419e7-117">Text value</span></span>

<span data-ttu-id="419e7-118">Une valeur de texte qui représente une valeur Boolean est requise si cet élément est présent.</span><span class="sxs-lookup"><span data-stu-id="419e7-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="419e7-119">La valeur **true** indique que le dossier peut être supprimé ; la valeur **false** signifie que le dossier ne peut pas être supprimé.</span><span class="sxs-lookup"><span data-stu-id="419e7-119">A value of **true** indicates that the folder can be deleted; a value of **false** means that the folder cannot be deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="419e7-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="419e7-120">Remarks</span></span>

<span data-ttu-id="419e7-121">Pour supprimer un dossier géré, utilisez l' [opération DeleteFolder](deletefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="419e7-121">To delete a managed folder, use the [DeleteFolder operation](deletefolder-operation.md).</span></span>
  
<span data-ttu-id="419e7-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="419e7-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="419e7-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="419e7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="419e7-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="419e7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="419e7-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="419e7-125">Schema name</span></span>  <br/> |<span data-ttu-id="419e7-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="419e7-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="419e7-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="419e7-127">Validation file</span></span>  <br/> |<span data-ttu-id="419e7-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="419e7-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="419e7-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="419e7-129">Can be empty</span></span>  <br/> |<span data-ttu-id="419e7-130">False</span><span class="sxs-lookup"><span data-stu-id="419e7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="419e7-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="419e7-131">See also</span></span>



[<span data-ttu-id="419e7-132">Opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="419e7-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="419e7-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="419e7-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="419e7-134">Suppression des dossiers</span><span class="sxs-lookup"><span data-stu-id="419e7-134">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

