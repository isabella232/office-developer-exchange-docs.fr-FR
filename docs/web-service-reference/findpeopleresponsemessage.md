---
title: FindPeopleResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ba686738-e654-404d-ab54-83c71d030350
description: L’élément FindPeopleResponseMessage Spécifie le message de réponse pour une demande FindPeople.
ms.openlocfilehash: 205f20b26b5097d24de45c5a5f9681f3557a6f87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756423"
---
# <a name="findpeopleresponsemessage"></a><span data-ttu-id="8855a-103">FindPeopleResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8855a-103">FindPeopleResponseMessage</span></span>

<span data-ttu-id="8855a-104">L’élément **FindPeopleResponseMessage** Spécifie le message de réponse pour une demande **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="8855a-104">The **FindPeopleResponseMessage** element specifies the response message for a **FindPeople** request.</span></span> 
  
```XML
<FindPeopleResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <People/>
   <TotalNumberOfPeopleInView/>
</FindPeopleResponseMessage>
```

 <span data-ttu-id="8855a-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8855a-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8855a-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="8855a-106">Attributes and elements</span></span>

<span data-ttu-id="8855a-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="8855a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8855a-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="8855a-108">Attributes</span></span>

<span data-ttu-id="8855a-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="8855a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8855a-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="8855a-110">Child elements</span></span>

<span data-ttu-id="8855a-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [personnes](people.md) | [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)</span><span class="sxs-lookup"><span data-stu-id="8855a-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [People](people.md) | [TotalNumberOfPeopleInView](totalnumberofpeopleinview.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8855a-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="8855a-112">Parent elements</span></span>

[<span data-ttu-id="8855a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8855a-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="8855a-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="8855a-114">Remarks</span></span>

<span data-ttu-id="8855a-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="8855a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8855a-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="8855a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8855a-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="8855a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8855a-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="8855a-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8855a-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="8855a-119">Schema name</span></span>  <br/> |<span data-ttu-id="8855a-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="8855a-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8855a-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="8855a-121">Validation file</span></span>  <br/> |<span data-ttu-id="8855a-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8855a-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8855a-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="8855a-123">Can be empty</span></span>  <br/> |<span data-ttu-id="8855a-124">false</span><span class="sxs-lookup"><span data-stu-id="8855a-124">false</span></span>  <br/> |
   

