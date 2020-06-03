---
title: GetDiscoverySearchConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b84a4c6-cb0a-4bca-85b2-fec32227930b
description: L’élément GetDiscoverySearchConfigurationResponseMessage spécifie le message de réponse pour une demande GetDiscoverySearchConfiguration.
ms.openlocfilehash: 23d1c5b7a61a9161d7383ec8b38cd0ebbebfc8cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460973"
---
# <a name="getdiscoverysearchconfigurationresponsemessage"></a><span data-ttu-id="a6eca-103">GetDiscoverySearchConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a6eca-103">GetDiscoverySearchConfigurationResponseMessage</span></span>

<span data-ttu-id="a6eca-104">L’élément **GetDiscoverySearchConfigurationResponseMessage** spécifie le message de réponse pour une demande **GetDiscoverySearchConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="a6eca-104">The **GetDiscoverySearchConfigurationResponseMessage** element specifies the response message for a **GetDiscoverySearchConfiguration** request.</span></span> 
  
```XML
<GetDiscoverySearchConfigurationResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DiscoverySearchConfigurations/>
</GetDiscoverySearchConfigurationResponseMessage>
```

 <span data-ttu-id="a6eca-105">**GetDiscoverySearchConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a6eca-105">**GetDiscoverySearchConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6eca-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="a6eca-106">Attributes and elements</span></span>

<span data-ttu-id="a6eca-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="a6eca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6eca-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="a6eca-108">Attributes</span></span>

<span data-ttu-id="a6eca-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="a6eca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6eca-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="a6eca-110">Child elements</span></span>

<span data-ttu-id="a6eca-111">[MessageText](messagetext.md)  |  [ResponseCode](responsecode.md)  |  [DescriptiveLinkKey](descriptivelinkkey.md)  |  [Messagexml](messagexml.md)  |  [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span><span class="sxs-lookup"><span data-stu-id="a6eca-111">[MessageText](messagetext.md) | [ResponseCode](responsecode.md) | [DescriptiveLinkKey](descriptivelinkkey.md) | [MessageXml](messagexml.md) | [DiscoverySearchConfigurations](discoverysearchconfigurations.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a6eca-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="a6eca-112">Parent elements</span></span>

[<span data-ttu-id="a6eca-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a6eca-113">ResponseMessages</span></span>](responsemessages.md)
  
## <a name="remarks"></a><span data-ttu-id="a6eca-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="a6eca-114">Remarks</span></span>

<span data-ttu-id="a6eca-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="a6eca-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a6eca-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="a6eca-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6eca-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="a6eca-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6eca-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="a6eca-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a6eca-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="a6eca-119">Schema name</span></span>  <br/> |<span data-ttu-id="a6eca-120">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="a6eca-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a6eca-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="a6eca-121">Validation file</span></span>  <br/> |<span data-ttu-id="a6eca-122">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="a6eca-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a6eca-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="a6eca-123">Can be empty</span></span>  <br/> |<span data-ttu-id="a6eca-124">false</span><span class="sxs-lookup"><span data-stu-id="a6eca-124">false</span></span>  <br/> |
   

