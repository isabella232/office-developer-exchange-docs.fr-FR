---
title: GetUMPropertiesResponse (service Web de messagerie unifiée)
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
description: L’élément GetUMPropertiesResponse définit une réponse à une opération GetUMProperties (service Web de messagerie unifiée).
ms.openlocfilehash: 3247489a305c694c10764d7a0c6f02b1fad51ebf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459124"
---
# <a name="getumpropertiesresponse-um-web-service"></a><span data-ttu-id="dbdec-103">GetUMPropertiesResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="dbdec-103">GetUMPropertiesResponse (UM web service)</span></span>

<span data-ttu-id="dbdec-104">L’élément **GetUMPropertiesResponse** définit une réponse à une [opération GetUMProperties (service Web de messagerie unifiée)](getumproperties-operation-um-web-service.md) .</span><span class="sxs-lookup"><span data-stu-id="dbdec-104">The **GetUMPropertiesResponse** element defines a response to a [GetUMProperties operation (UM web service)](getumproperties-operation-um-web-service.md) request.</span></span> 
  
[<span data-ttu-id="dbdec-105">GetUMPropertiesResponse (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="dbdec-105">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)
  
```xml
<GetUMPropertiesResponse>
  <OofStatus/>
  <MissedCallNotificationEnabled/>
  <PlayOnPhoneDialString/>
  <TelephoneAccessNumbers/>
  <TelephoneAccessFolderEmail/>
</GetUMPropertiesResponse>
```

 <span data-ttu-id="dbdec-106">**UMProperties**</span><span class="sxs-lookup"><span data-stu-id="dbdec-106">**UMProperties**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dbdec-107">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="dbdec-107">Attributes and elements</span></span>

<span data-ttu-id="dbdec-108">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="dbdec-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbdec-109">Attributs</span><span class="sxs-lookup"><span data-stu-id="dbdec-109">Attributes</span></span>

<span data-ttu-id="dbdec-110">Aucune.</span><span class="sxs-lookup"><span data-stu-id="dbdec-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dbdec-111">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="dbdec-111">Child elements</span></span>

|<span data-ttu-id="dbdec-112">**Élément**</span><span class="sxs-lookup"><span data-stu-id="dbdec-112">**Element**</span></span>|<span data-ttu-id="dbdec-113">**Description**</span><span class="sxs-lookup"><span data-stu-id="dbdec-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbdec-114">MissedCallNotificationEnabled (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="dbdec-114">MissedCallNotificationEnabled (UM web service)</span></span>](missedcallnotificationenabled-um-web-service.md) <br/> |<span data-ttu-id="dbdec-115">Indique si les notifications d’appels manqués sont activées.</span><span class="sxs-lookup"><span data-stu-id="dbdec-115">Indicates whether missed call notifications are enabled.</span></span>  <br/> |
|[<span data-ttu-id="dbdec-116">PlayOnPhoneDialString (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="dbdec-116">PlayOnPhoneDialString (UM web service)</span></span>](playonphonedialstring-um-web-service.md) <br/> |<span data-ttu-id="dbdec-117">Contient la chaîne de numérotation par défaut à utiliser pour l' [opération PlayOnPhone (service Web de messagerie unifiée)](playonphone-operation-um-web-service.md) et l' [opération PlayOnPhoneGreeting (service Web de messagerie unifiée)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="dbdec-117">Contains the default dial string to use for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>  <br/> |
|[<span data-ttu-id="dbdec-118">TelephoneAccessNumbers (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="dbdec-118">TelephoneAccessNumbers (UM web service)</span></span>](telephoneaccessnumbers-um-web-service.md) <br/> |<span data-ttu-id="dbdec-119">Contient la liste des numéros de téléphone que l’utilisateur peut utiliser pour accéder à la messagerie unifiée via un téléphone.</span><span class="sxs-lookup"><span data-stu-id="dbdec-119">Contains the list of telephone numbers the user can use to access Unified Messaging via a telephone.</span></span>  <br/> |
|[<span data-ttu-id="dbdec-120">TelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="dbdec-120">TelephoneAccessFolderEmail (UM web service)</span></span>](telephoneaccessfolderemail-um-web-service.md) <br/> |<span data-ttu-id="dbdec-121">Contient l’identificateur du dossier de messagerie à partir duquel la messagerie unifiée lira les messages par téléphone.</span><span class="sxs-lookup"><span data-stu-id="dbdec-121">Contains the identifier for the e-mail folder from which Unified Messaging will read messages over the telephone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dbdec-122">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="dbdec-122">Parent elements</span></span>

<span data-ttu-id="dbdec-123">Aucun.</span><span class="sxs-lookup"><span data-stu-id="dbdec-123">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="dbdec-124">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="dbdec-124">Text value</span></span>

<span data-ttu-id="dbdec-125">Aucune.</span><span class="sxs-lookup"><span data-stu-id="dbdec-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbdec-126">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="dbdec-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbdec-127">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="dbdec-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="dbdec-128">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="dbdec-128">Schema Name</span></span>  <br/> |<span data-ttu-id="dbdec-129">Messages</span><span class="sxs-lookup"><span data-stu-id="dbdec-129">Messages</span></span>  <br/> |
|<span data-ttu-id="dbdec-130">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="dbdec-130">Validation File</span></span>  <br/> |<span data-ttu-id="dbdec-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="dbdec-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="dbdec-132">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="dbdec-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbdec-133">False</span><span class="sxs-lookup"><span data-stu-id="dbdec-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbdec-134">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="dbdec-134">See also</span></span>



[<span data-ttu-id="dbdec-135">Opération GetUMProperties (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="dbdec-135">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)

