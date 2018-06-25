---
title: GetUMPropertiesResponse (service web de messagerie unifiée)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMPropertiesResponse
api_type:
- schema
ms.assetid: fcd93ce5-7403-46a9-b46e-56d2ebdd2f79
description: L’élément GetUMPropertiesResponse définit une réponse à une demande de (service web de messagerie unifiée) opération GetUMProperties.
ms.openlocfilehash: c0df872ad6b8e6541fa750ab87f4c1e5f0118b00
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19827685"
---
# <a name="getumpropertiesresponse-um-web-service"></a><span data-ttu-id="15f38-103">GetUMPropertiesResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15f38-103">GetUMPropertiesResponse (UM web service)</span></span>

<span data-ttu-id="15f38-104">L’élément **GetUMPropertiesResponse** définit une réponse à une demande de [l’opération GetUMProperties (service web de messagerie unifiée)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="15f38-104">The **GetUMPropertiesResponse** element defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="15f38-105">GetUMPropertiesResponse (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15f38-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="15f38-106">**UMProperties**</span><span class="sxs-lookup"><span data-stu-id="15f38-106">**UMProperties**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15f38-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="15f38-107">Attributes and elements</span></span>

<span data-ttu-id="15f38-108">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="15f38-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15f38-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="15f38-109">Attributes</span></span>

<span data-ttu-id="15f38-110">Aucun.</span><span class="sxs-lookup"><span data-stu-id="15f38-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15f38-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="15f38-111">Child elements</span></span>

|<span data-ttu-id="15f38-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="15f38-112">**Element**</span></span>|<span data-ttu-id="15f38-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="15f38-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15f38-114">MissedCallNotificationEnabled (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15f38-114">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md) <br/> |<span data-ttu-id="15f38-115">Indique si les notifications d’appels manqués sont activées.</span><span class="sxs-lookup"><span data-stu-id="15f38-115">Indicates whether missed call notifications are enabled.</span></span>  <br/> |
|[<span data-ttu-id="15f38-116">PlayOnPhoneDialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15f38-116">PlayOnPhoneDialString (UM web service)</span></span>](playonphonedialstring-um-web-service.md) <br/> |<span data-ttu-id="15f38-117">Contient la chaîne de numérotation par défaut à utiliser pour [l’opération PlayOnPhone (service web de messagerie unifiée)](playonphone-operation-um-web-service.md) et [l’opération PlayOnPhoneGreeting (service web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="15f38-117">Contains the default dial string to use for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>  <br/> |
|[<span data-ttu-id="15f38-118">TelephoneAccessNumbers (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15f38-118">TelephoneAccessNumbers (UM web service)</span></span>](telephoneaccessnumbers-um-web-service.md) <br/> |<span data-ttu-id="15f38-119">Contient la liste des numéros de téléphone que l’utilisateur peut utiliser pour accéder à la messagerie unifiée par le biais d’un téléphone.</span><span class="sxs-lookup"><span data-stu-id="15f38-119">Contains the list of telephone numbers the user can use to access Unified Messaging via a telephone.</span></span>  <br/> |
|[<span data-ttu-id="15f38-120">TelephoneAccessFolderEmail (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15f38-120">TelephoneAccessFolderEmail (UM web service)</span></span>](telephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="15f38-121">Contient l’identificateur pour le dossier de courrier électronique à partir de laquelle la messagerie unifiée sera lire des messages par téléphone.</span><span class="sxs-lookup"><span data-stu-id="15f38-121">Contains the identifier for the e-mail folder from which Unified Messaging will read messages over the telephone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="15f38-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="15f38-122">Parent elements</span></span>

<span data-ttu-id="15f38-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="15f38-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="15f38-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="15f38-124">Text value</span></span>

<span data-ttu-id="15f38-125">Aucun.</span><span class="sxs-lookup"><span data-stu-id="15f38-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15f38-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="15f38-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15f38-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="15f38-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="15f38-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="15f38-128">Schema Name</span></span>  <br/> |<span data-ttu-id="15f38-129">Messages</span><span class="sxs-lookup"><span data-stu-id="15f38-129">Messages</span></span>  <br/> |
|<span data-ttu-id="15f38-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="15f38-130">Validation File</span></span>  <br/> |<span data-ttu-id="15f38-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="15f38-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="15f38-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="15f38-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="15f38-133">False</span><span class="sxs-lookup"><span data-stu-id="15f38-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15f38-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="15f38-134">See also</span></span>



[<span data-ttu-id="15f38-135">Opération GetUMProperties (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15f38-135">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)

