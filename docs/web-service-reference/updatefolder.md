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
description: L’élément UpdateFolder représente l’opération qui est utilisée pour mettre à jour les propriétés d’un dossier spécifié.
ms.openlocfilehash: 124ffd02a5ea2e7bf6f21cc7009dde08837906f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457045"
---
# <a name="updatefolder"></a><span data-ttu-id="418e0-103">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="418e0-103">UpdateFolder</span></span>

<span data-ttu-id="418e0-104">L’élément **UpdateFolder** représente l’opération qui est utilisée pour mettre à jour les propriétés d’un dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="418e0-104">The **UpdateFolder** element represents the operation that is used to update properties for a specified folder.</span></span> 
  
```xml
<UpdateFolder>
   <FolderChanges/>
</UpdateFolder>
```

 <span data-ttu-id="418e0-105">**UpdateFolderType**</span><span class="sxs-lookup"><span data-stu-id="418e0-105">**UpdateFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="418e0-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="418e0-106">Attributes and elements</span></span>

<span data-ttu-id="418e0-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="418e0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="418e0-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="418e0-108">Attributes</span></span>

<span data-ttu-id="418e0-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="418e0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="418e0-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="418e0-110">Child elements</span></span>

|<span data-ttu-id="418e0-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="418e0-111">**Element**</span></span>|<span data-ttu-id="418e0-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="418e0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="418e0-113">FolderChanges</span><span class="sxs-lookup"><span data-stu-id="418e0-113">FolderChanges</span></span>](folderchanges.md) <br/> |<span data-ttu-id="418e0-114">Contient une collection de modifications pour un dossier spécifié.</span><span class="sxs-lookup"><span data-stu-id="418e0-114">Contains a collection of changes for a specified folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="418e0-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="418e0-115">Parent elements</span></span>

<span data-ttu-id="418e0-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="418e0-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="418e0-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="418e0-117">Remarks</span></span>

<span data-ttu-id="418e0-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="418e0-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="418e0-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="418e0-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="418e0-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="418e0-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="418e0-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="418e0-121">Schema Name</span></span>  <br/> |<span data-ttu-id="418e0-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="418e0-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="418e0-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="418e0-123">Validation File</span></span>  <br/> |<span data-ttu-id="418e0-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="418e0-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="418e0-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="418e0-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="418e0-126">False</span><span class="sxs-lookup"><span data-stu-id="418e0-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="418e0-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="418e0-127">See also</span></span>



[<span data-ttu-id="418e0-128">Opération UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="418e0-128">UpdateFolder operation</span></span>](updatefolder-operation.md)

