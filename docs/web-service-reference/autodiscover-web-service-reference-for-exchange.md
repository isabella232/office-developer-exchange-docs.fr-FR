---
title: Référence de service web de découverte automatique pour Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a01124a8-a8cf-4b80-8625-d7ee05690bca
description: Rechercher du contenu de référence pour le service web de découverte automatique dans Exchange.
ms.openlocfilehash: 48ca4a93c2120079cb675eabbc460bf0e75570b2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755358"
---
# <a name="autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="e7307-103">Référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e7307-103">Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="e7307-104">Rechercher du contenu de référence pour le service web de découverte automatique dans Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7307-104">Find reference content for the Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="e7307-105">Le service web de découverte automatique fournit les informations de configuration que votre application utilise pour créer une connexion à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7307-105">The Autodiscover web service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="e7307-106">Vous pouvez utiliser une des options suivantes pour se connecter au service de découverte automatique :</span><span class="sxs-lookup"><span data-stu-id="e7307-106">You can use one of the following options to connect to Autodiscover:</span></span>
  
- <span data-ttu-id="e7307-107">Service de découverte automatique SOAP — pour les clients qui se connectent à des versions d’Exchange commençant par Exchange 2010, notamment Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e7307-107">SOAP Autodiscover service —Available to clients that connect to versions of Exchange starting with Exchange 2010, including Exchange Online.</span></span>
    
- <span data-ttu-id="e7307-108">« XML brut ancienne » service de découverte automatique (POX) — pour les clients qui se connectent à des versions d’Exchange commençant par Exchange 2007, notamment Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="e7307-108">"plain old XML" (POX) Autodiscover service — Available to clients that connect to versions of Exchange starting with Exchange 2007, including Exchange Online.</span></span> 
    
<span data-ttu-id="e7307-109">À la fois le protocole SOAP et le service de découverte automatique variole peuvent fournir les informations de configuration que votre client utilisera pour créer une connexion à un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="e7307-109">Both the SOAP and the POX Autodiscover service can provide the configuration information that your client will use to create a connection to an Exchange server.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e7307-110">Pour les versions d’Exchange commençant par Exchange 2010, il est recommandé que vous utilisez le service de découverte automatique SOAP au lieu du service de découverte automatique variole.</span><span class="sxs-lookup"><span data-stu-id="e7307-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="e7307-111">Le service de découverte automatique SOAP fournit des requêtes de paramètre Autodiscover groupées et un contrôle plus précis sur les paramètres sont retournés dans la réponse.</span><span class="sxs-lookup"><span data-stu-id="e7307-111">The SOAP Autodiscover service provides batched Autodiscover setting requests and more granular control over which settings are returned in the response.</span></span> 
  
<span data-ttu-id="e7307-112">Cette section contient des informations de référence pour le service de découverte automatique SOAP et le service de découverte automatique variole.</span><span class="sxs-lookup"><span data-stu-id="e7307-112">This section contains reference information for the SOAP Autodiscover service and the POX Autodiscover service.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="e7307-113">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="e7307-113">In this section</span></span>
<span data-ttu-id="e7307-114"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="e7307-114"></span></span>

- [<span data-ttu-id="e7307-115">SOAP de référence de service web de découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e7307-115">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
    
- [<span data-ttu-id="e7307-116">Référence de service web variole découverte automatique pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e7307-116">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="e7307-117">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="e7307-117">See also</span></span>

- [<span data-ttu-id="e7307-118">Référence des services web pour Exchange</span><span class="sxs-lookup"><span data-stu-id="e7307-118">Web services reference for Exchange</span></span>](web-services-reference-for-exchange.md)
- [<span data-ttu-id="e7307-119">Service de découverte automatique (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e7307-119">Autodiscover Service (SOAP)</span></span>](http://msdn.microsoft.com/library/e24d1a1f-0d20-4bd9-ae4c-9112ecacea78%28Office.15%29.aspx)
- [<span data-ttu-id="e7307-120">Service de découverte automatique (POX)</span><span class="sxs-lookup"><span data-stu-id="e7307-120">Autodiscover Service (POX)</span></span>](http://msdn.microsoft.com/library/13c54de3-a91c-4424-8732-99dd8f2162ec%28Office.15%29.aspx)
    
