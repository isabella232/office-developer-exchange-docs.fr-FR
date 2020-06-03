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
ms.openlocfilehash: 5fe16c276bdb0c5b3b73ca63099559d3e869db3e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461589"
---
# <a name="candelete"></a><span data-ttu-id="4fe1a-103">CanDelete</span><span class="sxs-lookup"><span data-stu-id="4fe1a-103">CanDelete</span></span>

<span data-ttu-id="4fe1a-104">L’élément **CanDelete** indique si un dossier géré peut être supprimé par un client.</span><span class="sxs-lookup"><span data-stu-id="4fe1a-104">The **CanDelete** element indicates whether a managed folder can be deleted by a customer.</span></span> 
  
```xml
<CanDelete/>
```

 <span data-ttu-id="4fe1a-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="4fe1a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4fe1a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4fe1a-106">Attributes and elements</span></span>

<span data-ttu-id="4fe1a-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4fe1a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4fe1a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4fe1a-108">Attributes</span></span>

<span data-ttu-id="4fe1a-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4fe1a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4fe1a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4fe1a-110">Child elements</span></span>

<span data-ttu-id="4fe1a-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4fe1a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4fe1a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4fe1a-112">Parent elements</span></span>

|<span data-ttu-id="4fe1a-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4fe1a-113">**Element**</span></span>|<span data-ttu-id="4fe1a-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="4fe1a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4fe1a-115">ManagedFolderInformation</span><span class="sxs-lookup"><span data-stu-id="4fe1a-115">ManagedFolderInformation</span></span>](managedfolderinformation.md) <br/> |<span data-ttu-id="4fe1a-116">Contient des informations sur un dossier géré.</span><span class="sxs-lookup"><span data-stu-id="4fe1a-116">Contains information about a managed folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4fe1a-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="4fe1a-117">Text value</span></span>

<span data-ttu-id="4fe1a-118">Une valeur de texte qui représente une valeur booléenne est requise si cet élément est présent.</span><span class="sxs-lookup"><span data-stu-id="4fe1a-118">A text value that represents a Boolean value is required if this element is present.</span></span> <span data-ttu-id="4fe1a-119">La valeur **true** indique que le dossier peut être supprimé ; la valeur **false** signifie que le dossier ne peut pas être supprimé.</span><span class="sxs-lookup"><span data-stu-id="4fe1a-119">A value of **true** indicates that the folder can be deleted; a value of **false** means that the folder cannot be deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="4fe1a-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="4fe1a-120">Remarks</span></span>

<span data-ttu-id="4fe1a-121">Pour supprimer un dossier géré, utilisez l' [opération DeleteFolder](deletefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4fe1a-121">To delete a managed folder, use the [DeleteFolder operation](deletefolder-operation.md).</span></span>
  
<span data-ttu-id="4fe1a-122">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="4fe1a-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4fe1a-123">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4fe1a-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4fe1a-124">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4fe1a-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4fe1a-125">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4fe1a-125">Schema name</span></span>  <br/> |<span data-ttu-id="4fe1a-126">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="4fe1a-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="4fe1a-127">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4fe1a-127">Validation file</span></span>  <br/> |<span data-ttu-id="4fe1a-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4fe1a-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4fe1a-129">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4fe1a-129">Can be empty</span></span>  <br/> |<span data-ttu-id="4fe1a-130">False</span><span class="sxs-lookup"><span data-stu-id="4fe1a-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4fe1a-131">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4fe1a-131">See also</span></span>



[<span data-ttu-id="4fe1a-132">Opération CreateManagedFolder</span><span class="sxs-lookup"><span data-stu-id="4fe1a-132">CreateManagedFolder operation</span></span>](createmanagedfolder-operation.md)


- [<span data-ttu-id="4fe1a-133">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4fe1a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="4fe1a-134">Suppression de dossiers</span><span class="sxs-lookup"><span data-stu-id="4fe1a-134">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

