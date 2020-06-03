---
title: Opérations de service Web de messagerie unifiée pour Exchange
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
description: Recherchez des informations de référence pour les opérations de service Web de messagerie unifiée dans Exchange.
ms.openlocfilehash: b13ca2fbc44846db0bc98b3961916ba5d0872310
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529713"
---
# <a name="unified-messaging-web-service-operations-for-exchange"></a><span data-ttu-id="15cec-103">Opérations de service Web de messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="15cec-103">Unified Messaging web service operations for Exchange</span></span>

<span data-ttu-id="15cec-104">Recherchez des informations de référence pour les opérations de service Web de messagerie unifiée dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="15cec-104">Find reference information for the Unified Messaging web service operations in Exchange.</span></span>
  
<span data-ttu-id="15cec-105">Le service Web de messagerie unifiée fournit de nombreuses opérations qui permettent aux applications clientes de lire et de modifier des propriétés de messagerie unifiée, de lire des messages vocaux, d’enregistrer des messages d’accueil et de dicter des éléments de boîte aux lettres sur des appareils de téléphonie.</span><span class="sxs-lookup"><span data-stu-id="15cec-105">The Unified Messaging web service provides many operations that enable client applications to read and change Unified Messaging properties, play voice mail messages, record greetings, and dictate mailbox items over telephony devices.</span></span> <span data-ttu-id="15cec-106">Les Articles de cette section fournissent des informations sur la structure globale des messages de demande et de réponse pour les opérations.</span><span class="sxs-lookup"><span data-stu-id="15cec-106">The articles in this section provide information about the overall structure of the request and response messages for the operations.</span></span> <span data-ttu-id="15cec-107">Ces articles fournissent des exemples qui montrent des structures de messages communes.</span><span class="sxs-lookup"><span data-stu-id="15cec-107">These articles provide examples that show common message structures.</span></span> <span data-ttu-id="15cec-108">Vous pouvez utiliser ces exemples pour en savoir plus sur ce que vous pouvez faire avec une demande de service Web de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="15cec-108">You can use these examples to learn about what you can do with a Unified Messaging web service request.</span></span>
  
> [!NOTE]
> <span data-ttu-id="15cec-109">Pour les versions d’Exchange commençant par Exchange 2010, nous vous recommandons d’utiliser les opérations de messagerie unifiée disponibles dans les [services Web Exchange (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) au lieu du service Web de messagerie unifiée, pour les raisons suivantes :</span><span class="sxs-lookup"><span data-stu-id="15cec-109">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the Unified Messaging web service, for the following reasons:</span></span> 
> - <span data-ttu-id="15cec-110">Les fonctionnalités de messagerie unifiée EWS ont une prise en charge de première classe dans l’API managée EWS.</span><span class="sxs-lookup"><span data-stu-id="15cec-110">The EWS-based Unified Messaging features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="15cec-111">Dans les versions d’Exchange à partir d’Exchange 2010, les nouvelles fonctionnalités de messagerie unifiée sont ajoutées à EWS, mais pas au service Web de messagerie unifiée.</span><span class="sxs-lookup"><span data-stu-id="15cec-111">In versions of Exchange starting with Exchange 2010, new Unified Messaging features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="15cec-112">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="15cec-112">In this section</span></span>
<span data-ttu-id="15cec-113"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="15cec-113"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="15cec-114">Opération de déconnexion (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-114">Disconnect operation (UM web service)</span></span>](disconnect-operation-um-web-service.md)    
- [<span data-ttu-id="15cec-115">Opération GetCallInfo (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-115">GetCallInfo operation (UM web service)</span></span>](getcallinfo-operation-um-web-service.md)   
- [<span data-ttu-id="15cec-116">Opération GetUMProperties (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-116">GetUMProperties operation (UM web service)</span></span>](getumproperties-operation-um-web-service.md)   
- [<span data-ttu-id="15cec-117">Opération IsUMEnabled (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-117">IsUMEnabled operation (UM web service)</span></span>](isumenabled-operation-um-web-service.md)   
- [<span data-ttu-id="15cec-118">Opération PlayOnPhone (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-118">PlayOnPhone operation (UM web service)</span></span>](playonphone-operation-um-web-service.md)   
- [<span data-ttu-id="15cec-119">Opération PlayOnPhoneGreeting (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-119">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)   
- [<span data-ttu-id="15cec-120">Opération ResetPIN (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-120">ResetPIN operation (UM web service)</span></span>](resetpin-operation-um-web-service.md)   
- [<span data-ttu-id="15cec-121">Opération SetMissedCallNotificationEnabled (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-121">SetMissedCallNotificationEnabled operation (UM web service)</span></span>](setmissedcallnotificationenabled-operation-um-web-service.md)  
- [<span data-ttu-id="15cec-122">Opération SetOofStatus (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-122">SetOofStatus operation (UM web service)</span></span>](setoofstatus-operation-um-web-service.md)    
- [<span data-ttu-id="15cec-123">Opération SetPlayOnPhoneDialString (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-123">SetPlayOnPhoneDialString operation (UM web service)</span></span>](setplayonphonedialstring-operation-um-web-service.md)   
- [<span data-ttu-id="15cec-124">Opération SetTelephoneAccessFolderEmail (service Web de messagerie unifiée)</span><span class="sxs-lookup"><span data-stu-id="15cec-124">SetTelephoneAccessFolderEmail operation (UM web service)</span></span>](settelephoneaccessfolderemail-operation-um-web-service.md)
    
## <a name="see-also"></a><span data-ttu-id="15cec-125">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="15cec-125">See also</span></span>

- [<span data-ttu-id="15cec-126">Référence du service Web de messagerie unifiée pour Exchange</span><span class="sxs-lookup"><span data-stu-id="15cec-126">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
- [<span data-ttu-id="15cec-127">Découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="15cec-127">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="15cec-128">Commencer à utiliser les services web dans Exchange</span><span class="sxs-lookup"><span data-stu-id="15cec-128">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

