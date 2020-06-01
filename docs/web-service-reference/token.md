---
title: Jeton
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Token
api_type:
- schema
ms.assetid: 62b700e1-88c7-41ef-b431-d7af4a8b54a7
description: L’élément Token contient des données chiffrées qui représentent le jeton d’identification pour les données partagées.
ms.openlocfilehash: c2e80082f9b4ecb96defdca8c5f0223a945661ba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458907"
---
# <a name="token"></a><span data-ttu-id="ebcc9-103">Jeton</span><span class="sxs-lookup"><span data-stu-id="ebcc9-103">Token</span></span>

<span data-ttu-id="ebcc9-104">L’élément **Token** contient des données chiffrées qui représentent le jeton d’identification pour les données partagées.</span><span class="sxs-lookup"><span data-stu-id="ebcc9-104">The **Token** element contains encrypted data that represents the identification token for the shared data.</span></span> 
  
```xml
<Token/>
```

 <span data-ttu-id="ebcc9-105">**EncryptedDataContainerType**</span><span class="sxs-lookup"><span data-stu-id="ebcc9-105">**EncryptedDataContainerType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ebcc9-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="ebcc9-106">Attributes and elements</span></span>

<span data-ttu-id="ebcc9-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="ebcc9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebcc9-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="ebcc9-108">Attributes</span></span>

<span data-ttu-id="ebcc9-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="ebcc9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebcc9-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="ebcc9-110">Child elements</span></span>

<span data-ttu-id="ebcc9-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="ebcc9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ebcc9-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="ebcc9-112">Parent elements</span></span>

|<span data-ttu-id="ebcc9-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="ebcc9-113">**Element**</span></span>|<span data-ttu-id="ebcc9-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="ebcc9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebcc9-115">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="ebcc9-115">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="ebcc9-116">Contient les données chiffrées qu’un client peut utiliser pour autoriser le partage de son calendrier ou des données de contact avec d’autres clients.</span><span class="sxs-lookup"><span data-stu-id="ebcc9-116">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ebcc9-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="ebcc9-117">Remarks</span></span>

<span data-ttu-id="ebcc9-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services Web Exchange de l’ordinateur qui exécute Microsoft Exchange Server sur lequel le rôle de serveur d’accès au client est installé.</span><span class="sxs-lookup"><span data-stu-id="ebcc9-118">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ebcc9-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="ebcc9-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebcc9-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="ebcc9-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ebcc9-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="ebcc9-121">Schema Name</span></span>  <br/> |<span data-ttu-id="ebcc9-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="ebcc9-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="ebcc9-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="ebcc9-123">Validation File</span></span>  <br/> |<span data-ttu-id="ebcc9-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ebcc9-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ebcc9-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="ebcc9-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="ebcc9-126">False</span><span class="sxs-lookup"><span data-stu-id="ebcc9-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ebcc9-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ebcc9-127">See also</span></span>



[<span data-ttu-id="ebcc9-128">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="ebcc9-128">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="ebcc9-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="ebcc9-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

