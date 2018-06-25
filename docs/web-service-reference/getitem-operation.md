---
title: GetItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e3590b8b-c2a7-4dad-a014-6360197b68e4
description: Pour des informations sur la EWS GetItem operation.
ms.openlocfilehash: 9b63032b2eaa3bf26027a42e38bfa06bedcbac86
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19756660"
---
# <a name="getitem-operation"></a><span data-ttu-id="ed725-103">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="ed725-103">GetItem operation</span></span>

<span data-ttu-id="ed725-104">Trouvez des informations sur l’opération EWS **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="ed725-104">Find information about the **GetItem** EWS operation.</span></span> 
  
<span data-ttu-id="ed725-105">L’opération **GetItem** Obtient les éléments à partir de la banque d’informations Exchange.</span><span class="sxs-lookup"><span data-stu-id="ed725-105">The **GetItem** operation gets items from the Exchange store.</span></span> 
  
## <a name="using-the-getitem-operation"></a><span data-ttu-id="ed725-106">Utilisation de l’opération GetItem</span><span class="sxs-lookup"><span data-stu-id="ed725-106">Using the GetItem operation</span></span>

<span data-ttu-id="ed725-107">L’opération **GetItem** renvoie plusieurs propriétés de l’élément.</span><span class="sxs-lookup"><span data-stu-id="ed725-107">The **GetItem** operation returns many item properties.</span></span> <span data-ttu-id="ed725-108">Les propriétés qui sont retournées dans une réponse **GetItem** varient en fonction de la forme demandée, des propriétés supplémentaires requises et le type d’élément renvoyé.</span><span class="sxs-lookup"><span data-stu-id="ed725-108">The properties that are returned in a **GetItem** response vary based on the requested shape, requested additional properties, and the type of item returned.</span></span> 
  
<span data-ttu-id="ed725-109">Éléments de [message](message-ex15websvcsotherref.md) représentent des messages électroniques et tous les autres éléments qui ne sont pas fortement typées dans le schéma Exchange Web Services (EWS).</span><span class="sxs-lookup"><span data-stu-id="ed725-109">[Message](message-ex15websvcsotherref.md) elements represent email messages and all other items that are not strongly typed by the Exchange Web Services (EWS) schema.</span></span> <span data-ttu-id="ed725-110">Éléments tels que IPM. Partage et IPM.InfoPath sont renvoyés en tant qu’éléments du [Message](message-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="ed725-110">Items such as IPM.Sharing and IPM.InfoPath are returned as [Message](message-ex15websvcsotherref.md) elements.</span></span> <span data-ttu-id="ed725-111">Exchange ne renvoie pas de [l’élément de base](item.md) des réponses.</span><span class="sxs-lookup"><span data-stu-id="ed725-111">Exchange does not return the base [Item](item.md) element in responses.</span></span> 
  
<span data-ttu-id="ed725-112">L’opération **GetItem** ne renvoie pas les pièces jointes.</span><span class="sxs-lookup"><span data-stu-id="ed725-112">The **GetItem** operation does not return attachments.</span></span> <span data-ttu-id="ed725-113">Il retourne les métadonnées relatives à un fichier ou un élément attaché.</span><span class="sxs-lookup"><span data-stu-id="ed725-113">It does return metadata about an attached item or file.</span></span> <span data-ttu-id="ed725-114">Pour renvoyer une pièce jointe, utilisez l' [opération GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ed725-114">To return an attachment, use the [GetAttachment operation](getattachment-operation.md).</span></span>
  
## <a name="getitem-operation-soap-headers"></a><span data-ttu-id="ed725-115">En-têtes SOAP GetItem opération</span><span class="sxs-lookup"><span data-stu-id="ed725-115">GetItem operation SOAP headers</span></span>

<span data-ttu-id="ed725-116">L’opération de **GetItem** peut utiliser les en-têtes SOAP qui sont répertoriés dans le tableau suivant.</span><span class="sxs-lookup"><span data-stu-id="ed725-116">The **GetItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="ed725-117">En-tête \*\*\*</span><span class="sxs-lookup"><span data-stu-id="ed725-117">****Header****</span></span>|<span data-ttu-id="ed725-118">****Element****</span><span class="sxs-lookup"><span data-stu-id="ed725-118">****Element****</span></span>|<span data-ttu-id="ed725-119">****Description****</span><span class="sxs-lookup"><span data-stu-id="ed725-119">****Description****</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ed725-120">**DateTimePrecision**</span><span class="sxs-lookup"><span data-stu-id="ed725-120">**DateTimePrecision**</span></span> <br/> |[<span data-ttu-id="ed725-121">DateTimePrecision</span><span class="sxs-lookup"><span data-stu-id="ed725-121">DateTimePrecision</span></span>](datetimeprecision.md) <br/> |<span data-ttu-id="ed725-122">Spécifie la résolution des valeurs de date/heure dans les réponses à partir du serveur, en secondes ou en millisecondes.</span><span class="sxs-lookup"><span data-stu-id="ed725-122">Specifies the resolution of data/time values in responses from the server, either in seconds or in milliseconds.</span></span>  <br/> |
|<span data-ttu-id="ed725-123">**Emprunt d’identité**</span><span class="sxs-lookup"><span data-stu-id="ed725-123">**Impersonation**</span></span> <br/> |[<span data-ttu-id="ed725-124">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="ed725-124">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ed725-125">Identifie l’utilisateur emprunte l’identité de l’application cliente.</span><span class="sxs-lookup"><span data-stu-id="ed725-125">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="ed725-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="ed725-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="ed725-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="ed725-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="ed725-128">Identifie la culture, comme défini dans RFC 3066, « Balises pour l’Identification des langues », à utiliser pour accéder à la boîte aux lettres.</span><span class="sxs-lookup"><span data-stu-id="ed725-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="ed725-129">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="ed725-129">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="ed725-130">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="ed725-130">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ed725-131">Identifie la version du schéma pour la requête d’opération.</span><span class="sxs-lookup"><span data-stu-id="ed725-131">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="ed725-132">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="ed725-132">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="ed725-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ed725-133">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ed725-134">Identifie la version du serveur qui a répondu à la demande.</span><span class="sxs-lookup"><span data-stu-id="ed725-134">Identifies the version of the server that responded to the request.</span></span>  <br/> |
|<span data-ttu-id="ed725-135">**TimeZoneContext**</span><span class="sxs-lookup"><span data-stu-id="ed725-135">**TimeZoneContext**</span></span> <br/> |[<span data-ttu-id="ed725-136">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="ed725-136">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="ed725-137">Identifie le fuseau horaire à utiliser pour toutes les réponses à partir du serveur.</span><span class="sxs-lookup"><span data-stu-id="ed725-137">Identifies the time zone to be used for all responses from the server.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="ed725-138">Contenu de cette section</span><span class="sxs-lookup"><span data-stu-id="ed725-138">In This Section</span></span>

[<span data-ttu-id="ed725-139">Opération de GetItem (e-mail)</span><span class="sxs-lookup"><span data-stu-id="ed725-139">GetItem operation (email message)</span></span>](getitem-operation-email-message.md)
  
[<span data-ttu-id="ed725-140">Opération de GetItem (élément de calendrier)</span><span class="sxs-lookup"><span data-stu-id="ed725-140">GetItem operation (calendar item)</span></span>](getitem-operation-calendar-item.md)
  
[<span data-ttu-id="ed725-141">Opération de GetItem (tâche)</span><span class="sxs-lookup"><span data-stu-id="ed725-141">GetItem operation (task)</span></span>](getitem-operation-task.md)
  
[<span data-ttu-id="ed725-142">Opération de GetItem (contacts)</span><span class="sxs-lookup"><span data-stu-id="ed725-142">GetItem operation (contact)</span></span>](getitem-operation-contact.md)
  
## <a name="see-also"></a><span data-ttu-id="ed725-143">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ed725-143">See also</span></span>



[<span data-ttu-id="ed725-144">Référence EWS pour Exchange</span><span class="sxs-lookup"><span data-stu-id="ed725-144">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

