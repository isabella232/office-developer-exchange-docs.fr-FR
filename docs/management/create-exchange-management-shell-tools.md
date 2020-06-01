---
title: Créer des outils d’environnement de commande Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46e4812f-37a8-449f-bd37-bc4a94605db9
description: Trouvez des informations pour commencer à créer des outils Exchange Management Shell pour Exchange.
ms.openlocfilehash: c6e11fa5b55aa514b12f4f52bc9346ac213d3781
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463726"
---
# <a name="create-exchange-management-shell-tools"></a><span data-ttu-id="d1900-103">Créer des outils d’environnement de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="d1900-103">Create Exchange Management Shell tools</span></span>

<span data-ttu-id="d1900-104">Trouvez des informations pour commencer à créer des outils Exchange Management Shell pour Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1900-104">Find information to get started creating Exchange Management Shell tools for Exchange.</span></span>

<span data-ttu-id="d1900-105">**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="d1900-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="d1900-106">L’environnement de ligne de commande Exchange Management Shell fournit un ensemble complet de commandes, basées sur la plateforme Windows PowerShell, pour la gestion d’Exchange Online, Exchange Online dans le cadre d’Office 365 ou d’une version locale d’Exchange à partir d’Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="d1900-106">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="d1900-107">Vous pouvez utiliser les commandes de l’environnement de commande Exchange Management Shell pour automatiser l’administration d’un serveur en exécutant directement les commandes ou en utilisant des scripts de commandes.</span><span class="sxs-lookup"><span data-stu-id="d1900-107">You can use Exchange Management Shell commands to automate the administration of a server by directly executing the commands, or by using command scripts.</span></span>
  
<span data-ttu-id="d1900-108">Si vous devez utiliser les commandes de l’environnement de commande Exchange Management Shell à partir d’une application d’hébergement, telle qu’une application administrative qui s’exécute sur l’ordinateur de bureau de l’administrateur ou via une application Web, vous pouvez appeler des applets de commande Exchange Management Shell à partir de votre application Visual Basic ou C# pour gérer un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="d1900-108">If you need to use Exchange Management Shell commands from within a hosting application, such as an administrative application that is running on the administrator's desktop or through a web-based application, you can call Exchange Management Shell cmdlets from within your Visual Basic or C# application to manage an Exchange server.</span></span>
  
## <a name="get-started-with-exchange-management-shell-tools"></a><span data-ttu-id="d1900-109">Prise en main des outils Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="d1900-109">Get started with Exchange Management Shell tools</span></span>
<span data-ttu-id="d1900-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span><span class="sxs-lookup"><span data-stu-id="d1900-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span></span>

<span data-ttu-id="d1900-111">Si vous êtes familiarisé avec la création d’applications hôtes Windows PowerShell et que vous souhaitez voir un exemple illustrant comment appeler les cmdlets Exchange Management Shell à partir d’une application, ou pour voir un exemple des types d’applications que vous pouvez créer à l’aide des cmdlets de l’environnement de commande Exchange Management Shell, voir [Get a list of mail Users using the Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span><span class="sxs-lookup"><span data-stu-id="d1900-111">If you are familiar with creating Windows PowerShell host applications and want to see an example that shows how to call the Exchange Management Shell cmdlets from an application, or to see an example of the types of applications that you can create by using the Exchange Management Shell cmdlets, see [Get a list of mail users by using the Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span></span>
  
<span data-ttu-id="d1900-112">Les cmdlets de l’environnement de ligne de commande Exchange Management Shell sont des extensions de Windows PowerShell, un interpréteur de ligne de commande basé sur des tâches et un langage de script conçu spécifiquement pour l’administration du système.</span><span class="sxs-lookup"><span data-stu-id="d1900-112">The Exchange Management Shell cmdlets are extensions to Windows PowerShell, a task-based command-line shell and scripting language that is designed specifically for system administration.</span></span> <span data-ttu-id="d1900-113">Windows PowerShell est basé sur .NET Framework et fournit une API orientée objet pour les développeurs d’applications pour les cmdlets, les fournisseurs et les hôtes.</span><span class="sxs-lookup"><span data-stu-id="d1900-113">Windows PowerShell is built on the .NET Framework, and provides an object-oriented API for cmdlet, provider, and host application developers.</span></span> <span data-ttu-id="d1900-114">Pour en savoir plus sur la programmation Windows PowerShell, consultez le [Kit de développement logiciel (SDK) Windows PowerShell](https://msdn.microsoft.com/library/dd835506%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d1900-114">To learn about Windows PowerShell programming, see the [Windows PowerShell SDK](https://msdn.microsoft.com/library/dd835506%28VS.85%29.aspx).</span></span>
  
<span data-ttu-id="d1900-115">Les cmdlets de l’environnement de commande Exchange Management Shell acceptent et renvoient des objets.</span><span class="sxs-lookup"><span data-stu-id="d1900-115">The Exchange Management Shell cmdlets accept and return objects.</span></span> <span data-ttu-id="d1900-116">Pour obtenir la liste des applets de commande Exchange Management Shell et leurs types d’entrée et de sortie, consultez la rubrique [types d’entrée et de sortie de la cmdlet Exchange Management Shell](exchange-management-shell-cmdlet-input-and-output-types.md).</span><span class="sxs-lookup"><span data-stu-id="d1900-116">For a list of Exchange management shell cmdlets and their input and output types, see [Exchange Management Shell cmdlet input and output types](exchange-management-shell-cmdlet-input-and-output-types.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="d1900-117">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="d1900-117">In this section</span></span>

- [<span data-ttu-id="d1900-118">Cmdlets Exchange Management Shell nouvelles et mises à jour</span><span class="sxs-lookup"><span data-stu-id="d1900-118">New and updated Exchange Management Shell cmdlets</span></span>](new-and-updated-exchange-management-shell-cmdlets.md)  
- [<span data-ttu-id="d1900-119">Types d’entrée et de sortie de la cmdlet d’Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="d1900-119">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
- [<span data-ttu-id="d1900-120">Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="d1900-120">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
- [<span data-ttu-id="d1900-121">Utiliser la réponse de cmdlet de l’environnement de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="d1900-121">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)


## <a name="see-also"></a><span data-ttu-id="d1900-122">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="d1900-122">See also</span></span>

- [<span data-ttu-id="d1900-123">Espaces de noms Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="d1900-123">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)  
- [<span data-ttu-id="d1900-124">Exchange Server PowerShell (environnement de commande Exchange Management Shell)</span><span class="sxs-lookup"><span data-stu-id="d1900-124">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)  
- [<span data-ttu-id="d1900-125">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="d1900-125">Windows PowerShell</span></span>](https://msdn.microsoft.com/library/dd835506%28v=vs.85%29.aspx)
    

