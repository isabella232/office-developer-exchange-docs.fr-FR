---
title: GetImItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 455e5709-6c06-49fd-bfb2-403fc912287c
description: L’élément de demande GetImItems définit une requête pour obtenir des informations sur les groupes de messagerie instantanées spécifiés et les personnages contacts de messagerie instantanée.
ms.openlocfilehash: ff7d520dde44fac6e9278633c1ad46b07b38d6c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756639"
---
# <a name="getimitems"></a><span data-ttu-id="382b6-103">GetImItems</span><span class="sxs-lookup"><span data-stu-id="382b6-103">GetImItems</span></span>

<span data-ttu-id="382b6-104">L’élément de demande **GetImItems** définit une requête pour obtenir des informations sur les groupes de messagerie instantanées spécifiés et les personnages contacts de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="382b6-104">The **GetImItems** request element defines a request to get information about the specified instant messaging groups and instant messaging contact personas.</span></span> 
  
```XML
<GetImItems>
   <ContactIds/>
   <GroupIds/>
   <ExtendedProperties/>
</GetImItems>
```

 <span data-ttu-id="382b6-105">**GetImItemsType**</span><span class="sxs-lookup"><span data-stu-id="382b6-105">**GetImItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="382b6-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="382b6-106">Attributes and elements</span></span>

<span data-ttu-id="382b6-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="382b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="382b6-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="382b6-108">Attributes</span></span>

<span data-ttu-id="382b6-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="382b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="382b6-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="382b6-110">Child elements</span></span>

<span data-ttu-id="382b6-111">[ContactIds](contactids.md) | [les GroupID](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span><span class="sxs-lookup"><span data-stu-id="382b6-111">[ContactIds](contactids.md) | [GroupIds](groupids.md) | [ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)](extendedproperties-nonemptyarrayofextendedfielduris.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="382b6-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="382b6-112">Parent elements</span></span>

<span data-ttu-id="382b6-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="382b6-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="382b6-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="382b6-114">Remarks</span></span>

<span data-ttu-id="382b6-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="382b6-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="382b6-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="382b6-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="382b6-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="382b6-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="382b6-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="382b6-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="382b6-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="382b6-119">Schema name</span></span>  <br/> |<span data-ttu-id="382b6-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="382b6-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="382b6-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="382b6-121">Validation file</span></span>  <br/> |<span data-ttu-id="382b6-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="382b6-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="382b6-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="382b6-123">Can be empty</span></span>  <br/> ||
   

