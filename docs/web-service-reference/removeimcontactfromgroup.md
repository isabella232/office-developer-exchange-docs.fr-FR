---
title: RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a62b0640-9800-45a6-a297-2105ff36881e
description: L’élément RemoveImContactFromGroup définit une demande pour supprimer un contact d’un groupe de messagerie instantané de la messagerie instantanée.
ms.openlocfilehash: 402cbd6929428d410ce5701b0c1afa901703bc29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829094"
---
# <a name="removeimcontactfromgroup"></a><span data-ttu-id="08352-103">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="08352-103">RemoveImContactFromGroup</span></span>

<span data-ttu-id="08352-104">L’élément **RemoveImContactFromGroup** définit une demande pour supprimer un contact d’un groupe de messagerie instantané de la messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="08352-104">The **RemoveImContactFromGroup** element defines a request to remove an instant messaging contact from an instant messaging group.</span></span> 
  
```XML
<RemoveImContactFromGroup>
   <ContactId/>
   <GroupId/>
</RemoveImContactFromGroup>
```

 <span data-ttu-id="08352-105">**RemoveImContactFromGroupType**</span><span class="sxs-lookup"><span data-stu-id="08352-105">**RemoveImContactFromGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08352-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="08352-106">Attributes and elements</span></span>

<span data-ttu-id="08352-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="08352-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08352-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="08352-108">Attributes</span></span>

<span data-ttu-id="08352-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08352-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08352-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="08352-110">Child elements</span></span>

<span data-ttu-id="08352-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="08352-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08352-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="08352-112">Parent elements</span></span>

<span data-ttu-id="08352-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="08352-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08352-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="08352-114">Remarks</span></span>

<span data-ttu-id="08352-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="08352-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="08352-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="08352-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08352-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="08352-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08352-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="08352-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="08352-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="08352-119">Schema name</span></span>  <br/> |<span data-ttu-id="08352-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="08352-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="08352-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="08352-121">Validation file</span></span>  <br/> |<span data-ttu-id="08352-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="08352-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="08352-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="08352-123">Can be empty</span></span>  <br/> ||
   

