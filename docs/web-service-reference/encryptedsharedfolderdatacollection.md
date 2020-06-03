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
description: L’élément EncryptedSharedFolderDataCollection contient une collection de structures de données qu’un client peut utiliser pour autoriser le partage de son calendrier ou des données de contact avec d’autres clients.
ms.openlocfilehash: e8ed9221952892abda7b4eac62b16cdc4976c6e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461267"
---
# <a name="encryptedsharedfolderdatacollection"></a><span data-ttu-id="dcbef-103">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="dcbef-103">EncryptedSharedFolderDataCollection</span></span>

<span data-ttu-id="dcbef-104">L’élément **EncryptedSharedFolderDataCollection** contient une collection de structures de données qu’un client peut utiliser pour autoriser le partage de son calendrier ou des données de contact avec d’autres clients.</span><span class="sxs-lookup"><span data-stu-id="dcbef-104">The **EncryptedSharedFolderDataCollection** element contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderDataCollection>   <EncryptedSharedFolderData/></EncryptedSharedFolderDataCollection>
```

 <span data-ttu-id="dcbef-105">**ArrayOfEncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="dcbef-105">**ArrayOfEncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dcbef-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dcbef-106">Attributes and elements</span></span>

<span data-ttu-id="dcbef-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dcbef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dcbef-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="dcbef-108">Attributes</span></span>

<span data-ttu-id="dcbef-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="dcbef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dcbef-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dcbef-110">Child elements</span></span>

|<span data-ttu-id="dcbef-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dcbef-111">**Element**</span></span>|<span data-ttu-id="dcbef-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="dcbef-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcbef-113">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="dcbef-113">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="dcbef-114">Contient les données chiffrées qu’un client peut utiliser pour autoriser le partage de son calendrier ou des données de contact avec d’autres clients.</span><span class="sxs-lookup"><span data-stu-id="dcbef-114">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dcbef-115">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dcbef-115">Parent elements</span></span>

|<span data-ttu-id="dcbef-116">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dcbef-116">**Element**</span></span>|<span data-ttu-id="dcbef-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="dcbef-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dcbef-118">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="dcbef-118">GetSharingMetadataResponse</span></span>](getsharingmetadataresponse.md) <br/> |<span data-ttu-id="dcbef-119">Définit une réponse à une demande de [Opération de GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dcbef-119">Defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="dcbef-120">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="dcbef-120">GetSharingMetadataResponseMessage</span></span>](getsharingmetadataresponsemessage.md) <br/> |<span data-ttu-id="dcbef-121">Contient l'état et les résultats d'une demande unique [Opération de GetSharingMetadata](getsharingmetadata-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="dcbef-121">Contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dcbef-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="dcbef-122">Remarks</span></span>

<span data-ttu-id="dcbef-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="dcbef-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dcbef-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dcbef-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dcbef-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dcbef-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dcbef-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dcbef-126">Schema Name</span></span>  <br/> |<span data-ttu-id="dcbef-127">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="dcbef-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="dcbef-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dcbef-128">Validation File</span></span>  <br/> |<span data-ttu-id="dcbef-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dcbef-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dcbef-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dcbef-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="dcbef-131">False</span><span class="sxs-lookup"><span data-stu-id="dcbef-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dcbef-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dcbef-132">See also</span></span>

- [<span data-ttu-id="dcbef-133">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="dcbef-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="dcbef-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="dcbef-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

