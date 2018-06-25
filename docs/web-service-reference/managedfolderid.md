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
ms.openlocfilehash: acdb69f82678633baff12c46494c39015c36d233
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19828340"
---
# <a name="managedfolderid"></a><span data-ttu-id="737fb-103">ManagedFolderId</span><span class="sxs-lookup"><span data-stu-id="737fb-103">ManagedFolderId</span></span>

<span data-ttu-id="737fb-104">L’élément **ManagedFolderId** contient l’ID de dossier du dossier géré.</span><span class="sxs-lookup"><span data-stu-id="737fb-104">The **ManagedFolderId** element contains the folder ID of the managed folder.</span></span> 
  
```xml
<ManagedFolderId/>
```

 <span data-ttu-id="737fb-105">**string**</span><span class="sxs-lookup"><span data-stu-id="737fb-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="737fb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="737fb-106">Attributes and elements</span></span>

<span data-ttu-id="737fb-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="737fb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="737fb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="737fb-108">Attributes</span></span>

<span data-ttu-id="737fb-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="737fb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="737fb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="737fb-110">Child elements</span></span>

<span data-ttu-id="737fb-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="737fb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="737fb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="737fb-112">Parent elements</span></span>

|<span data-ttu-id="737fb-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="737fb-113">**Element**</span></span>|<span data-ttu-id="737fb-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="737fb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="737fb-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="737fb-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="737fb-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="737fb-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="737fb-117">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="737fb-117">Text value</span></span>

<span data-ttu-id="737fb-118">Une valeur de texte est nécessaire pour cet élément.</span><span class="sxs-lookup"><span data-stu-id="737fb-118">A text value is required for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="737fb-119">Remarques</span><span class="sxs-lookup"><span data-stu-id="737fb-119">Remarks</span></span>

<span data-ttu-id="737fb-120">La valeur de l’identificateur **ManagedFolderId** est l’équivalent de la propriété **Guid** qui est extrait par le `Get-ManagedFolder` commande Microsoft Windows Powershell.</span><span class="sxs-lookup"><span data-stu-id="737fb-120">The **ManagedFolderId** identifier value is the equivalent of the **Guid** property that is retrieved by the  `Get-ManagedFolder` Microsoft Windows Powershell command.</span></span> <span data-ttu-id="737fb-121">Il est également la valeur de l’attribut **GUID d’objet** pour le dossier géré dans le service d’annuaire Active Directory.</span><span class="sxs-lookup"><span data-stu-id="737fb-121">It is also the value of the **objectGUID** attribute for the managed folder in the Active Directory directory service.</span></span> 
  
<span data-ttu-id="737fb-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="737fb-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="737fb-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="737fb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="737fb-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="737fb-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="737fb-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="737fb-125">Schema name</span></span>  <br/> |<span data-ttu-id="737fb-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="737fb-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="737fb-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="737fb-127">Validation file</span></span>  <br/> |<span data-ttu-id="737fb-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="737fb-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="737fb-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="737fb-129">Can be empty</span></span>  <br/> |<span data-ttu-id="737fb-130">False</span><span class="sxs-lookup"><span data-stu-id="737fb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="737fb-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="737fb-131">See also</span></span>



[<span data-ttu-id="737fb-132">Opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="737fb-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="737fb-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="737fb-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="737fb-134">Suppression des dossiers</span><span class="sxs-lookup"><span data-stu-id="737fb-134">Deleting Folders</span></span>](http://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)
  
[<span data-ttu-id="737fb-135">Ajout de dossiers gérés</span><span class="sxs-lookup"><span data-stu-id="737fb-135">Adding Managed Folders</span></span>](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

