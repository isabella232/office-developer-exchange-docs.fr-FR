---
title: Opérations du service web messagerie unifiées pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Unified
api_type:
- schema
ms.assetid: d92455bd-24e8-4255-9f93-2bdeff00d42d
description: Trouvez des informations de référence pour les opérations de service web de messagerie unifiée dans Exchange.
ms.openlocfilehash: 21d3469d752ff6cdca4ed4ea9151daca52d51e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19838799"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a><span data-ttu-id="7daa9-103">Opérations du service web messagerie unifiées pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7daa9-103">Unified Messaging web service operations for Exchange</span></span>

<span data-ttu-id="7daa9-104">Trouvez des informations de référence pour les opérations de service web de messagerie unifiée dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="7daa9-104">Find reference information for the Unified Messaging web service operations in Exchange.</span></span>
  
<span data-ttu-id="7daa9-105">Le service web de messagerie unifiée offre de nombreuses opérations qui permettent aux applications clientes lire et modifier les propriétés de la messagerie unifiée, lire des messages vocaux de voix, enregistrez le message d’accueil et déterminent les éléments de boîte aux lettres sur les périphériques de téléphonie.</span><span class="sxs-lookup"><span data-stu-id="7daa9-105">The Unified Messaging web service provides many operations that enable client applications to read and change Unified Messaging properties, play voice mail messages, record greetings, and dictate mailbox items over telephony devices.</span></span> <span data-ttu-id="7daa9-106">Les articles de cette section fournissent des informations sur la structure globale des messages pour les opérations de requête et de réponse.</span><span class="sxs-lookup"><span data-stu-id="7daa9-106">The articles in this section provide information about the overall structure of the request and response messages for the operations.</span></span> <span data-ttu-id="7daa9-107">Ces articles fournissent des exemples qui montrent les structures de message communes.</span><span class="sxs-lookup"><span data-stu-id="7daa9-107">These articles provide examples that show common message structures.</span></span> <span data-ttu-id="7daa9-108">Vous pouvez utiliser ces exemples pour en savoir plus sur ce que vous pouvez faire avec une demande de service web de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="7daa9-108">You can use these examples to learn about what you can do with a Unified Messaging web service request.</span></span>
  
> [!NOTE]
>  <span data-ttu-id="7daa9-109">Pour les versions d’Exchange commençant par Exchange 2010, nous recommandons d’utiliser les opérations de la messagerie unifiée qui sont disponibles dans [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) au lieu du service web de messagerie unifiée, pour les raisons suivantes : > basée sur le EWS Fonctionnalités de messagerie unifiées ont la prise en charge de première classe dans l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="7daa9-109">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the Unified Messaging web service, for the following reasons: >  The EWS-based Unified Messaging features have first-class support in the EWS Managed API.</span></span> <span data-ttu-id="7daa9-110">> Dans les versions d’Exchange commençant par Exchange 2010, les nouvelles fonctionnalités de messagerie unifiée sont ajoutées pour EWS mais pas pour le service web de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="7daa9-110">>  In versions of Exchange starting with Exchange 2010, new Unified Messaging features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="7daa9-111">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="7daa9-111">In this section</span></span>
<span data-ttu-id="7daa9-112"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="7daa9-112"></span></span>

- [<span data-ttu-id="7daa9-113">(Service web de messagerie unifiée) de l’opération de déconnexion</span><span class="sxs-lookup"><span data-stu-id="7daa9-113">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-114">Opération GetCallInfo (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-114">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-115">Opération GetUMProperties (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-115">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-116">Opération IsUMEnabled (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-116">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-117">Opération PlayOnPhone (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-117">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-118">Opération PlayOnPhoneGreeting (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-118">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-119">Opération ResetPIN (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-119">ResetPIN operation (UM web service)</span></span>](resetpin-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-120">Opération SetMissedCallNotificationEnabled (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-120">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-121">Opération SetOofStatus (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-121">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-122">Opération SetPlayOnPhoneDialString (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-122">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)
    
- [<span data-ttu-id="7daa9-123">Opération SetTelephoneAccessFolderEmail (service web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="7daa9-123">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a><span data-ttu-id="7daa9-124">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="7daa9-124">See also</span></span>

- [<span data-ttu-id="7daa9-125">Référence au service web messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7daa9-125">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
- [<span data-ttu-id="7daa9-126">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="7daa9-126">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="7daa9-127">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="7daa9-127">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

