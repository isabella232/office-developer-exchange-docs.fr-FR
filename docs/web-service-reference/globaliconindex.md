---
title: GlobalIconIndex
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d28ed70-4cfe-46e4-8d15-593c6e355bcf
description: L’élément GlobalIconIndex identifie l’index de l’icône global pour tous les éléments dans une conversation.
ms.openlocfilehash: e8d78bfcfc0e57df9230db86e080d1ee29878094
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19827727"
---
# <a name="globaliconindex"></a><span data-ttu-id="c4903-103">GlobalIconIndex</span><span class="sxs-lookup"><span data-stu-id="c4903-103">GlobalIconIndex</span></span>

<span data-ttu-id="c4903-104">L’élément **GlobalIconIndex** identifie l’index de l’icône global pour tous les éléments dans une conversation.</span><span class="sxs-lookup"><span data-stu-id="c4903-104">The **GlobalIconIndex** element identifies the global icon index for all items in a conversation.</span></span> 
  
```XML
<IconIndex>Default | PostItem | MailRead | MailUnread | MailReplied | MailForwarded | MailEncrypted | MailSmimeSigned | MailEncrytedReplied | MailSmimeSignedReplied | MailEncryptedForwarded | MailSmimeSignedForwarded | MailEncryptedRead | MailSmimeSignedRead | MailIrm | MaillrmForwarded | MaillrmReplied | SmsSubmitted | SmsRoutedToDeliveryPoint | SmsRoutedToExternalMessagingSystem | SmsDelivered | OutlookDefaultForContacts | AppointmentItem | AppointmentRecur | AppointmentMeet | AppointmentMeetRecur | AppointmentMeetNY | AppointmentMeetYes | AppointmentMeetNo | AppointmentMeetMaybe | AppointmentMeetCancel | AppointmentMeetInfo | TaskItem | TaskRecur | TaskOwned | TaskDelegated</IconIndex>
```

 <span data-ttu-id="c4903-105">**IconIndexType**</span><span class="sxs-lookup"><span data-stu-id="c4903-105">**IconIndexType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4903-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="c4903-106">Attributes and elements</span></span>

<span data-ttu-id="c4903-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="c4903-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4903-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="c4903-108">Attributes</span></span>

<span data-ttu-id="c4903-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4903-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4903-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="c4903-110">Child elements</span></span>

<span data-ttu-id="c4903-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="c4903-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c4903-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="c4903-112">Parent elements</span></span>

<span data-ttu-id="c4903-113">[Conversation (ConversationType)](conversation-conversationtype.md) | [élément](item.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [tâche ](task.md)</span><span class="sxs-lookup"><span data-stu-id="c4903-113">[Conversation (ConversationType)](conversation-conversationtype.md) | [Item](item.md) | [Contact](contact.md) | [DistributionList](distributionlist.md) | [Message](message-ex15websvcsotherref.md) | [CalendarItem](calendaritem.md) | [PostItem](postitem.md) | [Task](task.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c4903-114">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="c4903-114">Text value</span></span>

<span data-ttu-id="c4903-115">Le tableau suivant contient les valeurs de texte possibles pour l’élément **GlobalIconIndex** .</span><span class="sxs-lookup"><span data-stu-id="c4903-115">The following table contains the possible text values for the **GlobalIconIndex** element.</span></span> 
  
|<span data-ttu-id="c4903-116">**Valeur**</span><span class="sxs-lookup"><span data-stu-id="c4903-116">**Value**</span></span>|<span data-ttu-id="c4903-117">**Description**</span><span class="sxs-lookup"><span data-stu-id="c4903-117">**Description**</span></span>|
|:-----|:-----|
|||
|<span data-ttu-id="c4903-118">Default (Défaut)</span><span class="sxs-lookup"><span data-stu-id="c4903-118">Default</span></span>  <br/> |<span data-ttu-id="c4903-119">Spécifie l’icône par défaut.</span><span class="sxs-lookup"><span data-stu-id="c4903-119">Specifies the default icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-120">Objet postItem</span><span class="sxs-lookup"><span data-stu-id="c4903-120">PostItem</span></span>  <br/> |<span data-ttu-id="c4903-121">Spécifie l’icône pour un élément de publication.</span><span class="sxs-lookup"><span data-stu-id="c4903-121">Specifies the icon for a post item.</span></span>  <br/> |
|<span data-ttu-id="c4903-122">MailRead</span><span class="sxs-lookup"><span data-stu-id="c4903-122">MailRead</span></span>  <br/> |<span data-ttu-id="c4903-123">Spécifie que le message lu icône.</span><span class="sxs-lookup"><span data-stu-id="c4903-123">Specifies the mail read icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-124">MailUnread</span><span class="sxs-lookup"><span data-stu-id="c4903-124">MailUnread</span></span>  <br/> |<span data-ttu-id="c4903-125">Spécifie l’icône Courrier non lu.</span><span class="sxs-lookup"><span data-stu-id="c4903-125">Specifies the unread mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-126">MailReplied</span><span class="sxs-lookup"><span data-stu-id="c4903-126">MailReplied</span></span>  <br/> |<span data-ttu-id="c4903-127">Spécifie la réponse à l’icône Courrier.</span><span class="sxs-lookup"><span data-stu-id="c4903-127">Specifies the replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-128">MailForwarded</span><span class="sxs-lookup"><span data-stu-id="c4903-128">MailForwarded</span></span>  <br/> |<span data-ttu-id="c4903-129">Spécifie l’icône Courrier transféré.</span><span class="sxs-lookup"><span data-stu-id="c4903-129">Specifies the forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-130">MailEncrypted</span><span class="sxs-lookup"><span data-stu-id="c4903-130">MailEncrypted</span></span>  <br/> |<span data-ttu-id="c4903-131">Spécifie l’icône message chiffré.</span><span class="sxs-lookup"><span data-stu-id="c4903-131">Specifies the encrypted mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-132">MailSmimeSigned</span><span class="sxs-lookup"><span data-stu-id="c4903-132">MailSmimeSigned</span></span>  <br/> |<span data-ttu-id="c4903-133">Spécifie l’icône de messages électroniques signés Secure/Multipurpose Internet Mail Extensions (S/MIME).</span><span class="sxs-lookup"><span data-stu-id="c4903-133">Specifies the Secure/Multipurpose Internet Mail Extensions (S/MIME) signed mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-134">MailEncryptedReplied</span><span class="sxs-lookup"><span data-stu-id="c4903-134">MailEncryptedReplied</span></span>  <br/> |<span data-ttu-id="c4903-135">Spécifie qu'une réponse chiffrés à l’icône Courrier.</span><span class="sxs-lookup"><span data-stu-id="c4903-135">Specifies the encrypted replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-136">MailSmimeSignedReplied</span><span class="sxs-lookup"><span data-stu-id="c4903-136">MailSmimeSignedReplied</span></span>  <br/> |<span data-ttu-id="c4903-137">Spécifie que le S/MIME signés répondu à l’icône Courrier.</span><span class="sxs-lookup"><span data-stu-id="c4903-137">Specifies the S/MIME signed replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-138">MailEncryptedForwarded</span><span class="sxs-lookup"><span data-stu-id="c4903-138">MailEncryptedForwarded</span></span>  <br/> |<span data-ttu-id="c4903-139">Spécifie l’icône Courrier transféré chiffré.</span><span class="sxs-lookup"><span data-stu-id="c4903-139">Specifies the encrypted forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-140">MailSmimeSignedForwarded</span><span class="sxs-lookup"><span data-stu-id="c4903-140">MailSmimeSignedForwarded</span></span>  <br/> |<span data-ttu-id="c4903-141">Spécifie le S/MIME signé transféré icône Courrier.</span><span class="sxs-lookup"><span data-stu-id="c4903-141">Specifies the S/MIME signed forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-142">MailEncryptedRead</span><span class="sxs-lookup"><span data-stu-id="c4903-142">MailEncryptedRead</span></span>  <br/> |<span data-ttu-id="c4903-143">Spécifie l’icône message lecture chiffré.</span><span class="sxs-lookup"><span data-stu-id="c4903-143">Specifies the encrypted read mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-144">MailSmimeSignedRead</span><span class="sxs-lookup"><span data-stu-id="c4903-144">MailSmimeSignedRead</span></span>  <br/> |<span data-ttu-id="c4903-145">Spécifie le S/MIME signé lire l’icône Courrier.</span><span class="sxs-lookup"><span data-stu-id="c4903-145">Specifies the S/MIME signed read mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-146">MailIrm</span><span class="sxs-lookup"><span data-stu-id="c4903-146">MailIrm</span></span>  <br/> |<span data-ttu-id="c4903-147">Spécifie l’icône Courrier protégés par IRM Information Rights Management.</span><span class="sxs-lookup"><span data-stu-id="c4903-147">Specifies the Information Rights Management (IRM)-protected mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-148">MailIrmForwarded</span><span class="sxs-lookup"><span data-stu-id="c4903-148">MailIrmForwarded</span></span>  <br/> |<span data-ttu-id="c4903-149">Spécifie le-protégé par IRM transféré icône Courrier.</span><span class="sxs-lookup"><span data-stu-id="c4903-149">Specifies the IRM-protected forwarded mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-150">MailIrmReplied</span><span class="sxs-lookup"><span data-stu-id="c4903-150">MailIrmReplied</span></span>  <br/> |<span data-ttu-id="c4903-151">Spécifie que le-protégé par IRM a répondu à l’icône Courrier.</span><span class="sxs-lookup"><span data-stu-id="c4903-151">Specifies the IRM-protected replied to mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-152">SmsSubmitted</span><span class="sxs-lookup"><span data-stu-id="c4903-152">SmsSubmitted</span></span>  <br/> |<span data-ttu-id="c4903-153">Spécifie l’icône pour le courrier électronique envoyé pour le routage du Service SMS (Short Message).</span><span class="sxs-lookup"><span data-stu-id="c4903-153">Specifies the icon for mail submitted for Short Message Service (SMS) routing.</span></span>  <br/> |
|<span data-ttu-id="c4903-154">SmsRoutedToDeliveryPoint</span><span class="sxs-lookup"><span data-stu-id="c4903-154">SmsRoutedToDeliveryPoint</span></span>  <br/> |<span data-ttu-id="c4903-155">Spécifie l’icône pour le routage de SMS vers un point de remise externe.</span><span class="sxs-lookup"><span data-stu-id="c4903-155">Specifies the icon for SMS routing to an external delivery point.</span></span>  <br/> |
|<span data-ttu-id="c4903-156">SmsRoutedToExternalMessagingSystem</span><span class="sxs-lookup"><span data-stu-id="c4903-156">SmsRoutedToExternalMessagingSystem</span></span>  <br/> |<span data-ttu-id="c4903-157">Spécifie l’icône pour le routage de SMS vers un système de messagerie externe.</span><span class="sxs-lookup"><span data-stu-id="c4903-157">Specifies the icon for SMS routing to an external messaging system.</span></span>  <br/> |
|<span data-ttu-id="c4903-158">SmsDelivered</span><span class="sxs-lookup"><span data-stu-id="c4903-158">SmsDelivered</span></span>  <br/> |<span data-ttu-id="c4903-159">Spécifie l’icône de courrier remis SMS.</span><span class="sxs-lookup"><span data-stu-id="c4903-159">Specifies the SMS delivered mail icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-160">OutlookDefaultForContacts</span><span class="sxs-lookup"><span data-stu-id="c4903-160">OutlookDefaultForContacts</span></span>  <br/> |<span data-ttu-id="c4903-161">Spécifie l’icône par défaut pour les contacts.</span><span class="sxs-lookup"><span data-stu-id="c4903-161">Specifies the default icon for contacts.</span></span>  <br/> |
|<span data-ttu-id="c4903-162">Objet AppointmentItem</span><span class="sxs-lookup"><span data-stu-id="c4903-162">AppointmentItem</span></span>  <br/> |<span data-ttu-id="c4903-163">Spécifie l’icône de l’élément de rendez-vous.</span><span class="sxs-lookup"><span data-stu-id="c4903-163">Specifies the appointment item icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-164">AppointmentRecur</span><span class="sxs-lookup"><span data-stu-id="c4903-164">AppointmentRecur</span></span>  <br/> |<span data-ttu-id="c4903-165">Spécifie l’icône de rendez-vous périodiques.</span><span class="sxs-lookup"><span data-stu-id="c4903-165">Specifies the recurring appointment icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-166">AppointmentMeet</span><span class="sxs-lookup"><span data-stu-id="c4903-166">AppointmentMeet</span></span>  <br/> |<span data-ttu-id="c4903-167">Spécifie l’icône de réunion.</span><span class="sxs-lookup"><span data-stu-id="c4903-167">Specifies the meeting icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-168">AppointmentMeetRecur</span><span class="sxs-lookup"><span data-stu-id="c4903-168">AppointmentMeetRecur</span></span>  <br/> |<span data-ttu-id="c4903-169">Spécifie l’icône réunion périodique.</span><span class="sxs-lookup"><span data-stu-id="c4903-169">Specifies the recurring meeting icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-170">AppointmentMeetNY</span><span class="sxs-lookup"><span data-stu-id="c4903-170">AppointmentMeetNY</span></span>  <br/> |<span data-ttu-id="c4903-171">Spécifie l’icône d’une réponse provisoire à la réunion.</span><span class="sxs-lookup"><span data-stu-id="c4903-171">Specifies the icon for a tentative response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="c4903-172">AppointmentMeetYes</span><span class="sxs-lookup"><span data-stu-id="c4903-172">AppointmentMeetYes</span></span>  <br/> |<span data-ttu-id="c4903-173">Spécifie la réunion icône acceptation.</span><span class="sxs-lookup"><span data-stu-id="c4903-173">Specifies the meeting acceptance icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-174">AppointmentMeetNo</span><span class="sxs-lookup"><span data-stu-id="c4903-174">AppointmentMeetNo</span></span>  <br/> |<span data-ttu-id="c4903-175">Spécifie l’icône de réunion refusée.</span><span class="sxs-lookup"><span data-stu-id="c4903-175">Specifies the meeting declined icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-176">AppointmentMeetMaybe</span><span class="sxs-lookup"><span data-stu-id="c4903-176">AppointmentMeetMaybe</span></span>  <br/> |<span data-ttu-id="c4903-177">Spécifie l’icône d’une réponse peut-être à la réunion.</span><span class="sxs-lookup"><span data-stu-id="c4903-177">Specifies the icon for a maybe response to the meeting.</span></span>  <br/> |
|<span data-ttu-id="c4903-178">AppointmentMeetCancel</span><span class="sxs-lookup"><span data-stu-id="c4903-178">AppointmentMeetCancel</span></span>  <br/> |<span data-ttu-id="c4903-179">Spécifie la réunion annuler l’icône.</span><span class="sxs-lookup"><span data-stu-id="c4903-179">Specifies the meeting cancel icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-180">AppointmentMeetInfo</span><span class="sxs-lookup"><span data-stu-id="c4903-180">AppointmentMeetInfo</span></span>  <br/> |<span data-ttu-id="c4903-181">Spécifie la réunion icône d’information.</span><span class="sxs-lookup"><span data-stu-id="c4903-181">Specifies the meeting information icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-182">Objet TaskItem</span><span class="sxs-lookup"><span data-stu-id="c4903-182">TaskItem</span></span>  <br/> |<span data-ttu-id="c4903-183">Spécifie l’icône de l’élément de tâche.</span><span class="sxs-lookup"><span data-stu-id="c4903-183">Specifies the task item icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-184">TaskRecur</span><span class="sxs-lookup"><span data-stu-id="c4903-184">TaskRecur</span></span>  <br/> |<span data-ttu-id="c4903-185">Spécifie l’icône de la tâche périodique.</span><span class="sxs-lookup"><span data-stu-id="c4903-185">Specifies the recurring task icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-186">TaskOwned</span><span class="sxs-lookup"><span data-stu-id="c4903-186">TaskOwned</span></span>  <br/> |<span data-ttu-id="c4903-187">Spécifie la tâche propriétée d’icône.</span><span class="sxs-lookup"><span data-stu-id="c4903-187">Specifies the task owned icon.</span></span>  <br/> |
|<span data-ttu-id="c4903-188">TaskDelegated</span><span class="sxs-lookup"><span data-stu-id="c4903-188">TaskDelegated</span></span>  <br/> |<span data-ttu-id="c4903-189">Spécifie l’icône déléguées à ces tâches.</span><span class="sxs-lookup"><span data-stu-id="c4903-189">Specifies the task delegated icon.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c4903-190">Remarques</span><span class="sxs-lookup"><span data-stu-id="c4903-190">Remarks</span></span>

<span data-ttu-id="c4903-191">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c4903-191">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c4903-192">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="c4903-192">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c4903-193">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="c4903-193">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4903-194">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="c4903-194">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c4903-195">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="c4903-195">Schema name</span></span>  <br/> |<span data-ttu-id="c4903-196">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="c4903-196">Types schema</span></span>  <br/> |
|<span data-ttu-id="c4903-197">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="c4903-197">Validation file</span></span>  <br/> |<span data-ttu-id="c4903-198">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c4903-198">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c4903-199">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="c4903-199">Can be empty</span></span>  <br/> |<span data-ttu-id="c4903-200">false</span><span class="sxs-lookup"><span data-stu-id="c4903-200">false</span></span>  <br/> |
   

