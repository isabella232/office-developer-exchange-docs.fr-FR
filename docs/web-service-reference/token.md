---
title: Émission de jeton
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
description: L’élément jeton contient des données chiffrées qui représente le jeton d’identification pour les données partagées.
ms.openlocfilehash: cec11d9f2c24a250483c5be6e273f981fdf0a8e6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19838745"
---
# <a name="token"></a><span data-ttu-id="d80a7-103">Émission de jeton</span><span class="sxs-lookup"><span data-stu-id="d80a7-103">Token</span></span>

<span data-ttu-id="d80a7-104">L’élément **jeton** contient des données chiffrées qui représente le jeton d’identification pour les données partagées.</span><span class="sxs-lookup"><span data-stu-id="d80a7-104">The **Token** element contains encrypted data that represents the identification token for the shared data.</span></span> 
  
```xml
<Token/>
```

 <span data-ttu-id="d80a7-105">**EncryptedDataContainerType**</span><span class="sxs-lookup"><span data-stu-id="d80a7-105">**EncryptedDataContainerType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d80a7-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="d80a7-106">Attributes and elements</span></span>

<span data-ttu-id="d80a7-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="d80a7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d80a7-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="d80a7-108">Attributes</span></span>

<span data-ttu-id="d80a7-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d80a7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d80a7-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="d80a7-110">Child elements</span></span>

<span data-ttu-id="d80a7-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="d80a7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d80a7-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="d80a7-112">Parent elements</span></span>

|<span data-ttu-id="d80a7-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="d80a7-113">**Element**</span></span>|<span data-ttu-id="d80a7-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="d80a7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d80a7-115">EncryptedSharedFolderData</span><span class="sxs-lookup"><span data-stu-id="d80a7-115">EncryptedSharedFolderData</span></span>](encryptedsharedfolderdata.md) <br/> |<span data-ttu-id="d80a7-116">Contient les données chiffrées qu’un client peut utiliser pour autoriser le partage de son calendrier de données ou de contacts avec les autres clients.</span><span class="sxs-lookup"><span data-stu-id="d80a7-116">Contains the encrypted data that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d80a7-117">Remarques</span><span class="sxs-lookup"><span data-stu-id="d80a7-117">Remarks</span></span>

<span data-ttu-id="d80a7-118">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS que héberge Exchange Web Services de l’ordinateur qui exécute Microsoft Exchange Server qui a le rôle de serveur d’accès au Client est installé.</span><span class="sxs-lookup"><span data-stu-id="d80a7-118">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d80a7-119">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="d80a7-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d80a7-120">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="d80a7-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d80a7-121">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="d80a7-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d80a7-122">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="d80a7-122">Types schema</span></span>  <br/> |
|<span data-ttu-id="d80a7-123">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="d80a7-123">Validation File</span></span>  <br/> |<span data-ttu-id="d80a7-124">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d80a7-124">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d80a7-125">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="d80a7-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d80a7-126">False</span><span class="sxs-lookup"><span data-stu-id="d80a7-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d80a7-127">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d80a7-127">See also</span></span>



[<span data-ttu-id="d80a7-128">Opération de GetSharingMetadata</span><span class="sxs-lookup"><span data-stu-id="d80a7-128">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="d80a7-129">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="d80a7-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

