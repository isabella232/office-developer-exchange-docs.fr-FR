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
description: L’élément EncryptedSharedFolderData contient les données chiffrées qu’un client peut utiliser pour autoriser le partage de son calendrier ou des données de contact avec d’autres clients.
ms.openlocfilehash: 52e91eaf1ded31602b11e50c1b62159f72c101cd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530662"
---
# <a name="encryptedsharedfolderdata"></a><span data-ttu-id="85ed8-103">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="85ed8-103">EncryptedSharedFolderData</span></span>

<span data-ttu-id="85ed8-104">L’élément **EncryptedSharedFolderData** contient les données chiffrées qu’un client peut utiliser pour autoriser le partage de son calendrier ou des données de contact avec d’autres clients.</span><span class="sxs-lookup"><span data-stu-id="85ed8-104">The **EncryptedSharedFolderData** element contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span> 
  
```xml
<EncryptedSharedFolderData>   <Token/>   <Data/></EncryptedSharedFolderData>
```

 <span data-ttu-id="85ed8-105">**EncryptedSharedFolderDataType**</span><span class="sxs-lookup"><span data-stu-id="85ed8-105">**EncryptedSharedFolderDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85ed8-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="85ed8-106">Attributes and elements</span></span>

<span data-ttu-id="85ed8-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="85ed8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85ed8-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="85ed8-108">Attributes</span></span>

<span data-ttu-id="85ed8-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="85ed8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85ed8-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="85ed8-110">Child elements</span></span>

|<span data-ttu-id="85ed8-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85ed8-111">**Element**</span></span>|<span data-ttu-id="85ed8-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="85ed8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85ed8-113">Jeton</span><span class="sxs-lookup"><span data-stu-id="85ed8-113">Token</span></span>](token.md) <br/> |<span data-ttu-id="85ed8-114">Contient des données chiffrées qui représentent le jeton d’identification pour les données partagées.</span><span class="sxs-lookup"><span data-stu-id="85ed8-114">Contains encrypted data that represents the identification token for the shared data.</span></span>  <br/> |
|[<span data-ttu-id="85ed8-115">Données</span><span class="sxs-lookup"><span data-stu-id="85ed8-115">Data</span></span>](data.md) <br/> |<span data-ttu-id="85ed8-116">Contient des données chiffrées qui représentent les données partagées.</span><span class="sxs-lookup"><span data-stu-id="85ed8-116">Contains encrypted data that represents the shared data.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85ed8-117">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="85ed8-117">Parent elements</span></span>

|<span data-ttu-id="85ed8-118">**Élément**</span><span class="sxs-lookup"><span data-stu-id="85ed8-118">**Element**</span></span>|<span data-ttu-id="85ed8-119">**Description**</span><span class="sxs-lookup"><span data-stu-id="85ed8-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85ed8-120">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="85ed8-120">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="85ed8-121">Représente une collection de structures de données qu’un client peut utiliser pour autoriser le partage de son calendrier ou des données de contact avec d’autres clients.</span><span class="sxs-lookup"><span data-stu-id="85ed8-121">Represents a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="85ed8-122">Remarques</span><span class="sxs-lookup"><span data-stu-id="85ed8-122">Remarks</span></span>

<span data-ttu-id="85ed8-123">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="85ed8-123">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85ed8-124">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="85ed8-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85ed8-125">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="85ed8-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85ed8-126">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="85ed8-126">Schema Name</span></span>  <br/> |<span data-ttu-id="85ed8-127">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="85ed8-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="85ed8-128">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="85ed8-128">Validation File</span></span>  <br/> |<span data-ttu-id="85ed8-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="85ed8-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85ed8-130">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="85ed8-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="85ed8-131">False</span><span class="sxs-lookup"><span data-stu-id="85ed8-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85ed8-132">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="85ed8-132">See also</span></span>

- [<span data-ttu-id="85ed8-133">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="85ed8-133">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="85ed8-134">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="85ed8-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

