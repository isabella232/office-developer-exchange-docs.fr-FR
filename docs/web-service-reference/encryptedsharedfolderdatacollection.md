---
title: EncryptedSharedFolderDataCollection
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderDataCollection
api_type:
- schema
ms.assetid: 25c6ae87-bbb9-4dd5-a85a-d669fcea137f
description: L’élément EncryptedSharedFolderDataCollection contient une collection de structures de données qu’un client peut utiliser pour autoriser le partage de son calendrier de données ou de contacts avec les autres clients.
ms.openlocfilehash: e4d37f5df10f5e270be5126479485239f2205d6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756157"
---
# <a name="encryptedsharedfolderdatacollection"></a><span data-ttu-id="67843-103">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="67843-103">EncryptedSharedFolderDataCollection</span></span>

<span data-ttu-id="67843-104">L’élément **EncryptedSharedFolderDataCollection** contient une collection de structures de données qu’un client peut utiliser pour autoriser le partage de son calendrier de données ou de contacts avec les autres clients.</span><span class="sxs-lookup"><span data-stu-id="67843-104">The **EncryptedSharedFolderDataCollection** element contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 <span data-ttu-id="67843-105">**ArrayOfEncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="67843-105">**ArrayOfEncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="67843-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="67843-106">Attributes and elements</span></span>

<span data-ttu-id="67843-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="67843-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="67843-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="67843-108">Attributes</span></span>

<span data-ttu-id="67843-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="67843-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="67843-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="67843-110">Child elements</span></span>

|<span data-ttu-id="67843-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="67843-111">**Element**</span></span>|<span data-ttu-id="67843-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="67843-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67843-113">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="67843-113">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="67843-114">Contient les données chiffrées qu’un client peut utiliser pour autoriser le partage de son calendrier de données ou de contacts avec les autres clients.</span><span class="sxs-lookup"><span data-stu-id="67843-114">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="67843-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="67843-115">Parent elements</span></span>

|<span data-ttu-id="67843-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="67843-116">**Element**</span></span>|<span data-ttu-id="67843-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="67843-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="67843-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="67843-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="67843-119">Définit une réponse à une demande de [Opération de GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="67843-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="67843-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="67843-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="67843-121">Contient l'état et les résultats d'une demande unique [Opération de GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="67843-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="67843-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="67843-122">Remarks</span></span>

<span data-ttu-id="67843-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="67843-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="67843-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="67843-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="67843-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="67843-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="67843-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="67843-126">Schema Name</span></span>  <br/> |<span data-ttu-id="67843-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="67843-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="67843-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="67843-128">Validation File</span></span>  <br/> |<span data-ttu-id="67843-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="67843-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="67843-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="67843-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="67843-131">False</span><span class="sxs-lookup"><span data-stu-id="67843-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="67843-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="67843-132">See also</span></span>

- [<span data-ttu-id="67843-133">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="67843-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="67843-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="67843-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

