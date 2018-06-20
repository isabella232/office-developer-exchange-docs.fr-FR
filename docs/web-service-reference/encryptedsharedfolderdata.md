---
title: EncryptedSharedFolderData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EncryptedSharedFolderData
api_type:
- schema
ms.assetid: c1d4ca18-c5ce-41ff-bab4-f75e358c8b9f
description: L’élément EncryptedSharedFolderData contient les données chiffrées qu’un client peut utiliser pour autoriser le partage de son calendrier de données ou de contacts avec les autres clients.
ms.openlocfilehash: 63966e95becaab4b3b1e54aa81f1b20a8b09dfd3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19756159"
---
# <a name="encryptedsharedfolderdata"></a><span data-ttu-id="c243b-103">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="c243b-103">EncryptedSharedFolderData</span></span>

<span data-ttu-id="c243b-104">L’élément **EncryptedSharedFolderData** contient les données chiffrées qu’un client peut utiliser pour autoriser le partage de son calendrier de données ou de contacts avec les autres clients.</span><span class="sxs-lookup"><span data-stu-id="c243b-104">The **EncryptedSharedFolderData** element contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 <span data-ttu-id="c243b-105">**EncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="c243b-105">**EncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c243b-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c243b-106">Attributes and elements</span></span>

<span data-ttu-id="c243b-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c243b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c243b-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c243b-108">Attributes</span></span>

<span data-ttu-id="c243b-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c243b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c243b-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c243b-110">Child elements</span></span>

|<span data-ttu-id="c243b-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c243b-111">**Element**</span></span>|<span data-ttu-id="c243b-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="c243b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c243b-113">Jeton</span><span class="sxs-lookup"><span data-stu-id="c243b-113">Token</span></span>](token.md) <br/> |<span data-ttu-id="c243b-114">Contient des données chiffrées qui représente le jeton d’identification pour les données partagées.</span><span class="sxs-lookup"><span data-stu-id="c243b-114">Contains encrypted data that represents the identification token for the shared data.</span></span>  <br/> |
|[<span data-ttu-id="c243b-115">Data</span><span class="sxs-lookup"><span data-stu-id="c243b-115">Data</span></span>](data.md) <br/> |<span data-ttu-id="c243b-116">Contient des données chiffrées qui représente les données partagées.</span><span class="sxs-lookup"><span data-stu-id="c243b-116">Contains encrypted data that represents the shared data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c243b-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c243b-117">Parent elements</span></span>

|<span data-ttu-id="c243b-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="c243b-118">**Element**</span></span>|<span data-ttu-id="c243b-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="c243b-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c243b-120">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="c243b-120">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="c243b-121">Représente une collection de structures de données qu’un client peut utiliser pour autoriser le partage de son calendrier de données ou de contacts avec les autres clients.</span><span class="sxs-lookup"><span data-stu-id="c243b-121">Represents a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c243b-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="c243b-122">Remarks</span></span>

<span data-ttu-id="c243b-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="c243b-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c243b-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c243b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c243b-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c243b-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c243b-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c243b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="c243b-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c243b-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="c243b-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c243b-128">Validation File</span></span>  <br/> |<span data-ttu-id="c243b-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c243b-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c243b-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c243b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="c243b-131">False</span><span class="sxs-lookup"><span data-stu-id="c243b-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c243b-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c243b-132">See also</span></span>

- [<span data-ttu-id="c243b-133">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="c243b-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="c243b-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="c243b-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

