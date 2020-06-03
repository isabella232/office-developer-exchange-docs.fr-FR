---
title: ManagedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderId
api_type:
- schema
ms.assetid: 3efb7abb-0e91-4d8a-9fa2-3dec8bd17c30
description: L’élément ManagedFolderId contient l’ID de dossier du dossier géré.
ms.openlocfilehash: eacfe580342e6667fd9fc84ad953a5e4070b6ed7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465820"
---
# <a name="managedfolderid"></a><span data-ttu-id="f27fa-103">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="f27fa-103">ManagedFolderId</span></span>

<span data-ttu-id="f27fa-104">L’élément **ManagedFolderId** contient l’ID de dossier du dossier géré.</span><span class="sxs-lookup"><span data-stu-id="f27fa-104">The **ManagedFolderId** element contains the folder ID of the managed folder.</span></span> 
  
```xml
<ManagedFolderId/>
```

 <span data-ttu-id="f27fa-105">**chaîne**</span><span class="sxs-lookup"><span data-stu-id="f27fa-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f27fa-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="f27fa-106">Attributes and elements</span></span>

<span data-ttu-id="f27fa-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="f27fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f27fa-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="f27fa-108">Attributes</span></span>

<span data-ttu-id="f27fa-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="f27fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f27fa-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="f27fa-110">Child elements</span></span>

<span data-ttu-id="f27fa-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="f27fa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f27fa-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="f27fa-112">Parent elements</span></span>

|<span data-ttu-id="f27fa-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="f27fa-113">**Element**</span></span>|<span data-ttu-id="f27fa-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="f27fa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f27fa-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="f27fa-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="f27fa-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="f27fa-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f27fa-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="f27fa-117">Text value</span></span>

<span data-ttu-id="f27fa-118">Une valeur de texte est requise pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="f27fa-118">A text value is required for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f27fa-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="f27fa-119">Remarks</span></span>

<span data-ttu-id="f27fa-120">La valeur de l’identificateur **ManagedFolderId** est l’équivalent de la propriété **GUID** qui est extraite par la `Get-ManagedFolder` commande Microsoft Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f27fa-120">The **ManagedFolderId** identifier value is the equivalent of the **Guid** property that is retrieved by the  `Get-ManagedFolder` Microsoft Windows Powershell command.</span></span> <span data-ttu-id="f27fa-121">Il s’agit également de la valeur de l’attribut **objectGUID** pour le dossier géré dans le service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f27fa-121">It is also the value of the **objectGUID** attribute for the managed folder in the Active Directory directory service.</span></span> 
  
<span data-ttu-id="f27fa-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="f27fa-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f27fa-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="f27fa-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f27fa-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="f27fa-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f27fa-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="f27fa-125">Schema name</span></span>  <br/> |<span data-ttu-id="f27fa-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="f27fa-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="f27fa-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="f27fa-127">Validation file</span></span>  <br/> |<span data-ttu-id="f27fa-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f27fa-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f27fa-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="f27fa-129">Can be empty</span></span>  <br/> |<span data-ttu-id="f27fa-130">False</span><span class="sxs-lookup"><span data-stu-id="f27fa-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f27fa-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="f27fa-131">See also</span></span>



[<span data-ttu-id="f27fa-132">Opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="f27fa-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="f27fa-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="f27fa-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f27fa-134">Suppression de dossiers</span><span class="sxs-lookup"><span data-stu-id="f27fa-134">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
  
[<span data-ttu-id="f27fa-135">Ajout de dossiers gérés</span><span class="sxs-lookup"><span data-stu-id="f27fa-135">Adding Managed Folders</span></span>](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

