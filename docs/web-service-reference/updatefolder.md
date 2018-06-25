---
title: UpdateFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateFolder
api_type:
- schema
ms.assetid: 412d0683-2819-40c5-a0ae-f613499a7b66
description: L’élément UpdateFolder représente l’opération qui sert à mettre à jour les propriétés d’un dossier spécifié.
ms.openlocfilehash: 9a86bf6b3b5917600b3b09f23b3ee4e9cdc0364f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838861"
---
# <a name="updatefolder"></a><span data-ttu-id="87941-103">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="87941-103">UpdateFolder</span></span>

<span data-ttu-id="87941-104">L’élément **UpdateFolder** représente l’opération qui sert à mettre à jour les propriétés d’un dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="87941-104">The **UpdateFolder** element represents the operation that is used to update properties for a specified folder.</span></span> 
  
```xml
<UpdateFolder>
   <FolderChanges/>
</UpdateFolder>
```

 <span data-ttu-id="87941-105">**UpdateFolderType**</span><span class="sxs-lookup"><span data-stu-id="87941-105">**UpdateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="87941-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="87941-106">Attributes and elements</span></span>

<span data-ttu-id="87941-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="87941-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="87941-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="87941-108">Attributes</span></span>

<span data-ttu-id="87941-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="87941-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="87941-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="87941-110">Child elements</span></span>

|<span data-ttu-id="87941-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="87941-111">**Element**</span></span>|<span data-ttu-id="87941-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="87941-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="87941-113">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="87941-113">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="87941-114">Contient une collection des modifications pour un dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="87941-114">Contains a collection of changes for a specified folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="87941-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="87941-115">Parent elements</span></span>

<span data-ttu-id="87941-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="87941-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="87941-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="87941-117">Remarks</span></span>

<span data-ttu-id="87941-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="87941-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="87941-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="87941-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="87941-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="87941-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="87941-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="87941-121">Schema Name</span></span>  <br/> |<span data-ttu-id="87941-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="87941-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="87941-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="87941-123">Validation File</span></span>  <br/> |<span data-ttu-id="87941-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="87941-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="87941-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="87941-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="87941-126">False</span><span class="sxs-lookup"><span data-stu-id="87941-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="87941-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="87941-127">See also</span></span>



[<span data-ttu-id="87941-128">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="87941-128">UpdateFolder operation</span></span>](updatefolder-operation.md)

