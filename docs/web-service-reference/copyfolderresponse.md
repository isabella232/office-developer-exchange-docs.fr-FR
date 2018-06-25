---
title: CopyFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponse
api_type:
- schema
ms.assetid: 5bfbb4d3-e2ed-4b84-96f7-2175f1947aed
description: L’élément CopyFolderResponse définit une réponse à une demande de CopyFolder.
ms.openlocfilehash: 2f95089b9cb61e9e0047d02968d59d483fd7cdba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19755666"
---
# <a name="copyfolderresponse"></a><span data-ttu-id="28891-103">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="28891-103">CopyFolderResponse</span></span>

<span data-ttu-id="28891-104">L’élément **CopyFolderResponse** définit une réponse à une demande de CopyFolder.</span><span class="sxs-lookup"><span data-stu-id="28891-104">The **CopyFolderResponse** element defines a response to a CopyFolder request.</span></span> 
  
```xml
<CopyFolderResponse>
   <ResponseMessages/>
</CopyFolderResponse>
```

 <span data-ttu-id="28891-105">**CopyFolderResponseType**</span><span class="sxs-lookup"><span data-stu-id="28891-105">**CopyFolderResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28891-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="28891-106">Attributes and elements</span></span>

<span data-ttu-id="28891-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="28891-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28891-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="28891-108">Attributes</span></span>

<span data-ttu-id="28891-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28891-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="28891-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="28891-110">Child elements</span></span>

|<span data-ttu-id="28891-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="28891-111">**Element**</span></span>|<span data-ttu-id="28891-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="28891-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28891-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="28891-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="28891-114">Contient les messages de réponse pour une demande de Services Web Exchange.</span><span class="sxs-lookup"><span data-stu-id="28891-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28891-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="28891-115">Parent elements</span></span>

<span data-ttu-id="28891-116">Aucun.</span><span class="sxs-lookup"><span data-stu-id="28891-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="28891-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="28891-117">Remarks</span></span>

<span data-ttu-id="28891-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel EWS de l'ordinateur qui exécute MicrosoftExchange Server 2007 pour lequel le rôle serveur d'accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="28891-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28891-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="28891-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28891-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="28891-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28891-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="28891-121">Schema name</span></span>  <br/> |<span data-ttu-id="28891-122">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="28891-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28891-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="28891-123">Validation file</span></span>  <br/> |<span data-ttu-id="28891-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="28891-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28891-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="28891-125">Can be empty</span></span>  <br/> |<span data-ttu-id="28891-126">False</span><span class="sxs-lookup"><span data-stu-id="28891-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28891-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="28891-127">See also</span></span>



[<span data-ttu-id="28891-128">Opération CopyFolder</span><span class="sxs-lookup"><span data-stu-id="28891-128">CopyFolder operation</span></span>](copyfolder-operation.md)
  
[<span data-ttu-id="28891-129">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="28891-129">CopyFolder</span></span>](copyfolder.md)


- [<span data-ttu-id="28891-130">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="28891-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

