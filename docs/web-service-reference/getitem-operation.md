---
title: Opération GetItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Trouvez des informations sur l’opération EWS de GetItem.
localization_priority: Priority
ms.openlocfilehash: 8871dde183974454fc27dbddda489e6b0a70f3aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463327"
---
# <a name="getitem-operation"></a><span data-ttu-id="3d392-103">Opération GetItem</span><span class="sxs-lookup"><span data-stu-id="3d392-103">GetItem operation</span></span>

<span data-ttu-id="3d392-104">Trouvez des informations sur l’opération EWS de **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="3d392-104">Find information about the **GetItem** EWS operation.</span></span> 
  
<span data-ttu-id="3d392-105">L’opération **GetItem** obtient des éléments de la Banque d’Exchange.</span><span class="sxs-lookup"><span data-stu-id="3d392-105">The **GetItem** operation gets items from the Exchange store.</span></span> 
  
## <a name="using-the-getitem-operation"></a><span data-ttu-id="3d392-106">Utilisation de l’opération GetItem</span><span class="sxs-lookup"><span data-stu-id="3d392-106">Using the GetItem operation</span></span>

<span data-ttu-id="3d392-107">L’opération **GetItem** renvoie de nombreuses propriétés d’élément.</span><span class="sxs-lookup"><span data-stu-id="3d392-107">The **GetItem** operation returns many item properties.</span></span> <span data-ttu-id="3d392-108">Les propriétés renvoyées dans une réponse **GetItem** varient en fonction de la forme demandée, des propriétés supplémentaires demandées et du type d’élément renvoyé.</span><span class="sxs-lookup"><span data-stu-id="3d392-108">The properties that are returned in a **GetItem** response vary based on the requested shape, requested additional properties, and the type of item returned.</span></span> 
  
<span data-ttu-id="3d392-109">Les éléments de [message](message-ex15websvcsotherref.md) représentent les messages électroniques et tous les autres éléments qui ne sont pas fortement typés par le schéma des services Web Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="3d392-109">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="3d392-110">Des éléments tels que IPM. Le partage et IPM. InfoPath sont renvoyés en tant qu’éléments [message](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="3d392-110">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="3d392-111">Exchange ne retourne pas l’élément [élément](item.md) de base dans les réponses.</span><span class="sxs-lookup"><span data-stu-id="3d392-111">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="3d392-112">L’opération **GetItem** ne retourne pas les pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="3d392-112">The **GetItem** operation does not return attachments.</span></span> <span data-ttu-id="3d392-113">Elle renvoie les métadonnées d’un élément ou d’un fichier attaché.</span><span class="sxs-lookup"><span data-stu-id="3d392-113">It does return metadata about an attached item or file.</span></span> <span data-ttu-id="3d392-114">Pour renvoyer une pièce jointe, utilisez l' [opération GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3d392-114">To return an attachment, use the [GetAttachment operation](getattachment-operation.md).</span></span>
  
## <a name="getitem-operation-soap-headers"></a><span data-ttu-id="3d392-115">En-têtes SOAP d’opération GetItem</span><span class="sxs-lookup"><span data-stu-id="3d392-115">GetItem operation SOAP headers</span></span>

<span data-ttu-id="3d392-116">L’opération **GetItem** peut utiliser les en-têtes SOAP répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="3d392-116">The **GetItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="3d392-117">En-tête \* \* \* \*</span><span class="sxs-lookup"><span data-stu-id="3d392-117">\*\*\*\*Header\*\*\*\*</span></span>|<span data-ttu-id="3d392-118">\*\*\*\*Element\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="3d392-118">\*\*\*\*Element\*\*\*\*</span></span>|<span data-ttu-id="3d392-119">\*\*\*\*Description\*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="3d392-119">\*\*\*\*Description\*\*\*\*</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3d392-120">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="3d392-120">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="3d392-121">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="3d392-121">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="3d392-122">Spécifie la résolution des valeurs de données/temps dans les réponses du serveur, soit en secondes, soit en millisecondes.</span><span class="sxs-lookup"><span data-stu-id="3d392-122">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span>  <br/> |
|<span data-ttu-id="3d392-123">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="3d392-123">**Impersonation**</span></span> <br/> |[<span data-ttu-id="3d392-124">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="3d392-124">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="3d392-125">Identifie l’utilisateur qui emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="3d392-125">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="3d392-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="3d392-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="3d392-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="3d392-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="3d392-128">Identifie la culture, telle que définie dans la norme RFC 3066, « balises pour l’identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="3d392-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="3d392-129">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="3d392-129">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="3d392-130">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="3d392-130">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="3d392-131">Identifie la version de schéma de la demande d’opération.</span><span class="sxs-lookup"><span data-stu-id="3d392-131">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="3d392-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="3d392-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="3d392-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3d392-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3d392-134">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="3d392-134">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="3d392-135">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="3d392-135">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="3d392-136">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="3d392-136">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="3d392-137">Identifie le fuseau horaire à utiliser pour toutes les réponses du serveur.</span><span class="sxs-lookup"><span data-stu-id="3d392-137">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="3d392-138">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="3d392-138">In This Section</span></span>

[<span data-ttu-id="3d392-139">Opération GetItem (message électronique)</span><span class="sxs-lookup"><span data-stu-id="3d392-139">GetItem operation (email message)</span></span>](getitem-operation-email-message.md)
  
[<span data-ttu-id="3d392-140">Opération de GetItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="3d392-140">GetItem operation (calendar item)</span></span>](getitem-operation-calendar-item.md)
  
[<span data-ttu-id="3d392-141">Opération GetItem (tâche)</span><span class="sxs-lookup"><span data-stu-id="3d392-141">GetItem operation (task)</span></span>](getitem-operation-task.md)
  
[<span data-ttu-id="3d392-142">Opération GetItem (contact)</span><span class="sxs-lookup"><span data-stu-id="3d392-142">GetItem operation (contact)</span></span>](getitem-operation-contact.md)
  
## <a name="see-also"></a><span data-ttu-id="3d392-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="3d392-143">See also</span></span>



[<span data-ttu-id="3d392-144">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="3d392-144">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

