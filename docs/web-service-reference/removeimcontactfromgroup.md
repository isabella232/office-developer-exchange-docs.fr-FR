---
title: RemoveImContactFromGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a62b0640-9800-45a6-a297-2105ff36881e
description: L’élément RemoveImContactFromGroup définit une demande de suppression d’un contact de messagerie instantanée d’un groupe de messagerie instantanée.
ms.openlocfilehash: 379994ad5832b05e9f7da61d752f7660a6eec5ad
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466961"
---
# <a name="removeimcontactfromgroup"></a><span data-ttu-id="b76cb-103">RemoveImContactFromGroup</span><span class="sxs-lookup"><span data-stu-id="b76cb-103">RemoveImContactFromGroup</span></span>

<span data-ttu-id="b76cb-104">L’élément **RemoveImContactFromGroup** définit une demande de suppression d’un contact de messagerie instantanée d’un groupe de messagerie instantanée.</span><span class="sxs-lookup"><span data-stu-id="b76cb-104">The **RemoveImContactFromGroup** element defines a request to remove an instant messaging contact from an instant messaging group.</span></span> 
  
```XML
<RemoveImContactFromGroup>
   <ContactId/>
   <GroupId/>
</RemoveImContactFromGroup>
```

 <span data-ttu-id="b76cb-105">**RemoveImContactFromGroupType**</span><span class="sxs-lookup"><span data-stu-id="b76cb-105">**RemoveImContactFromGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b76cb-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="b76cb-106">Attributes and elements</span></span>

<span data-ttu-id="b76cb-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="b76cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b76cb-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="b76cb-108">Attributes</span></span>

<span data-ttu-id="b76cb-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="b76cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b76cb-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="b76cb-110">Child elements</span></span>

<span data-ttu-id="b76cb-111">[ContactID](contactid.md)  |  [GroupID](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="b76cb-111">[ContactId](contactid.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b76cb-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="b76cb-112">Parent elements</span></span>

<span data-ttu-id="b76cb-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="b76cb-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b76cb-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="b76cb-114">Remarks</span></span>

<span data-ttu-id="b76cb-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b76cb-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b76cb-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="b76cb-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b76cb-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="b76cb-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b76cb-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="b76cb-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b76cb-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="b76cb-119">Schema name</span></span>  <br/> |<span data-ttu-id="b76cb-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="b76cb-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b76cb-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="b76cb-121">Validation file</span></span>  <br/> |<span data-ttu-id="b76cb-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b76cb-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b76cb-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="b76cb-123">Can be empty</span></span>  <br/> ||
   

