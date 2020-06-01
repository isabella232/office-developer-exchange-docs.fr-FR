---
title: AddNewTelUriContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cff8ef19-3e19-4107-9b35-c8a2b87a41bc
description: L’élément AddNewTelUriContactToGroup spécifie les données d’entrée pour l’opération WSDL AddNewTelUriContactToGroup.
ms.openlocfilehash: 151c5b1dab7a3ffc9630fb4e4192b90bd1d4ae38
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464930"
---
# <a name="addnewteluricontacttogroup"></a><span data-ttu-id="20f00-103">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="20f00-103">AddNewTelUriContactToGroup</span></span>

<span data-ttu-id="20f00-104">L’élément **AddNewTelUriContactToGroup** spécifie les données d’entrée pour l’opération WSDL **AddNewTelUriContactToGroup** .</span><span class="sxs-lookup"><span data-stu-id="20f00-104">The **AddNewTelUriContactToGroup** element specifies the input data for the **AddNewTelUriContactToGroup** WSDL operation.</span></span> 
  
```XML
<AddNewTelUriContactToGroup>
   <TelUriAddress/>
   <ImContactSipUriAddress/>
   <ImTelephoneNumber/>
   <GroupId/>
</AddNewTelUriContactToGroup>
```

 <span data-ttu-id="20f00-105">**AddNewTelUriContactToGroupType**</span><span class="sxs-lookup"><span data-stu-id="20f00-105">**AddNewTelUriContactToGroupType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20f00-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="20f00-106">Attributes and elements</span></span>

<span data-ttu-id="20f00-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="20f00-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20f00-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="20f00-108">Attributes</span></span>

<span data-ttu-id="20f00-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="20f00-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20f00-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="20f00-110">Child elements</span></span>

<span data-ttu-id="20f00-111">[TelUriAddress](teluriaddress.md)  |  [ImContactSipUriAddress](imcontactsipuriaddress.md)  |  [ImTelephoneNumber](imtelephonenumber.md)  |  [GroupID](groupid.md)</span><span class="sxs-lookup"><span data-stu-id="20f00-111">[TelUriAddress](teluriaddress.md) | [ImContactSipUriAddress](imcontactsipuriaddress.md) | [ImTelephoneNumber](imtelephonenumber.md) | [GroupId](groupid.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20f00-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="20f00-112">Parent elements</span></span>

<span data-ttu-id="20f00-113">Aucun.</span><span class="sxs-lookup"><span data-stu-id="20f00-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="20f00-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="20f00-114">Remarks</span></span>

<span data-ttu-id="20f00-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="20f00-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="20f00-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="20f00-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20f00-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="20f00-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20f00-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="20f00-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="20f00-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="20f00-119">Schema name</span></span>  <br/> |<span data-ttu-id="20f00-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="20f00-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="20f00-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="20f00-121">Validation file</span></span>  <br/> |<span data-ttu-id="20f00-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="20f00-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="20f00-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="20f00-123">Can be empty</span></span>  <br/> |<span data-ttu-id="20f00-124">False</span><span class="sxs-lookup"><span data-stu-id="20f00-124">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="20f00-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="20f00-125">See also</span></span>

- [<span data-ttu-id="20f00-126">Opération AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="20f00-126">AddNewTelUriContactToGroup operation</span></span>](addnewteluricontacttogroup-operation.md)
- [<span data-ttu-id="20f00-127">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="20f00-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

