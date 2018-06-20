---
title: Créer des outils Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 46e4812f-37a8-449f-bd37-bc4a94605db9
description: Trouvez des informations pour commencer à créer des outils Exchange Management Shell pour Exchange.
ms.openlocfilehash: e8414460007f333e50c9d596bf977792977b1e4e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/11/2018
ms.locfileid: "19755074"
---
# <a name="create-exchange-management-shell-tools"></a><span data-ttu-id="60528-103">Créer des outils Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="60528-103">Create Exchange Management Shell tools</span></span>

<span data-ttu-id="60528-104">Trouvez des informations pour commencer à créer des outils Exchange Management Shell pour Exchange.</span><span class="sxs-lookup"><span data-stu-id="60528-104">Find information to get started creating Exchange Management Shell tools for Exchange.</span></span>

<span data-ttu-id="60528-105">**S’applique à :** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="60528-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="60528-106">Exchange Management Shell fournit un ensemble complet de commandes, en fonction de la plateforme de Windows PowerShell pour gérer Exchange Online, Exchange Online dans le cadre d’Office 365 ou une version locale d’Exchange commençant par Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="60528-106">The Exchange Management Shell provides a rich set of commands, based on the Windows PowerShell platform, for managing Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="60528-107">Vous pouvez utiliser les commandes Exchange Management Shell pour automatiser l’administration d’un serveur à l’exécution des commandes directement ou à l’aide de scripts de commandes.</span><span class="sxs-lookup"><span data-stu-id="60528-107">You can use Exchange Management Shell commands to automate the administration of a server by directly executing the commands, or by using command scripts.</span></span>
  
<span data-ttu-id="60528-108">Si vous devez utiliser les commandes Exchange Management Shell dans une application d’hébergement, comme une application d’administration qui s’exécute sur le bureau de l’administrateur ou via une application web, vous pouvez appeler les applets de commande Exchange Management Shell à partir de au sein de votre application Visual Basic ou c# pour gérer un serveur Exchange.</span><span class="sxs-lookup"><span data-stu-id="60528-108">If you need to use Exchange Management Shell commands from within a hosting application, such as an administrative application that is running on the administrator's desktop or through a web-based application, you can call Exchange Management Shell cmdlets from within your Visual Basic or C# application to manage an Exchange server.</span></span>
  
## <a name="get-started-with-exchange-management-shell-tools"></a><span data-ttu-id="60528-109">Prendre en main des outils Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="60528-109">Get started with Exchange Management Shell tools</span></span>
<span data-ttu-id="60528-110"><a name="SP15GettingStartedTemplate_WhatDoYouNeed"> </a></span><span class="sxs-lookup"><span data-stu-id="60528-110"></span></span>

<span data-ttu-id="60528-111">Si vous êtes familiarisé avec la création d’applications d’hébergement de Windows PowerShell et que vous souhaitez voir un exemple qui montre comment appeler les applets de commande Exchange Management Shell à partir d’une application, ou pour voir un exemple des types d’applications que vous pouvez créer à l’aide de la version d’Exchange Applets de commande Management Shell, voir [obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span><span class="sxs-lookup"><span data-stu-id="60528-111">If you are familiar with creating Windows PowerShell host applications and want to see an example that shows how to call the Exchange Management Shell cmdlets from an application, or to see an example of the types of applications that you can create by using the Exchange Management Shell cmdlets, see [Get a list of mail users by using the Exchange Management Shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md).</span></span>
  
<span data-ttu-id="60528-112">Les applets de commande Exchange Management Shell sont des extensions pour Windows PowerShell, un environnement de ligne de commande des tâches et langage de script qui est spécifiquement conçu pour l’administration système.</span><span class="sxs-lookup"><span data-stu-id="60528-112">The Exchange Management Shell cmdlets are extensions to Windows PowerShell, a task-based command-line shell and scripting language that is designed specifically for system administration.</span></span> <span data-ttu-id="60528-113">Windows PowerShell repose sur .NET Framework et fournit une API orientée objet pour l’applet de commande, le fournisseur et les développeurs d’applications hôte.</span><span class="sxs-lookup"><span data-stu-id="60528-113">Windows PowerShell is built on the .NET Framework, and provides an object-oriented API for cmdlet, provider, and host application developers.</span></span> <span data-ttu-id="60528-114">Pour plus d’informations sur la programmation de Windows PowerShell, voir le [Kit de développement Windows PowerShell](http://msdn.microsoft.com/en-us/library/dd835506%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="60528-114">To learn about Windows PowerShell programming, see the [Windows PowerShell SDK](http://msdn.microsoft.com/en-us/library/dd835506%28VS.85%29.aspx).</span></span>
  
<span data-ttu-id="60528-115">Les applets de commande Exchange Management Shell acceptent et retournent des objets.</span><span class="sxs-lookup"><span data-stu-id="60528-115">The Exchange Management Shell cmdlets accept and return objects.</span></span> <span data-ttu-id="60528-116">Pour obtenir la liste des applets de commande Exchange management shell et leurs types d’entrée et de sortie, voir [applet de commande Exchange Management Shell en entrée et sortie types](exchange-management-shell-cmdlet-input-and-output-types.md).</span><span class="sxs-lookup"><span data-stu-id="60528-116">For a list of Exchange management shell cmdlets and their input and output types, see [Exchange Management Shell cmdlet input and output types](exchange-management-shell-cmdlet-input-and-output-types.md).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="60528-117">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="60528-117">In this section</span></span>

- [<span data-ttu-id="60528-118">Nouveaux et mis à jour des applets de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="60528-118">New and updated Exchange Management Shell cmdlets</span></span>](new-and-updated-exchange-management-shell-cmdlets.md)  
- [<span data-ttu-id="60528-119">Entrée d’applet de commande Management Shell et types de sortie</span><span class="sxs-lookup"><span data-stu-id="60528-119">Exchange Management Shell cmdlet input and output types</span></span>](exchange-management-shell-cmdlet-input-and-output-types.md)
- [<span data-ttu-id="60528-120">Obtenir la liste des utilisateurs de messagerie à l’aide de l’environnement Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="60528-120">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
- [<span data-ttu-id="60528-121">Utilisation de la réponse d’applet de commande Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="60528-121">Use the Exchange Management Shell cmdlet response</span></span>](how-to-use-the-exchange-management-shell-cmdlet-response.md)


## <a name="see-also"></a><span data-ttu-id="60528-122">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="60528-122">See also</span></span>

- [<span data-ttu-id="60528-123">Espaces de noms Exchange Management Shell</span><span class="sxs-lookup"><span data-stu-id="60528-123">Exchange Management Shell namespaces</span></span>](exchange-management-shell-namespaces.md)  
- [<span data-ttu-id="60528-124">Exchange Server PowerShell (Exchange Management Shell)</span><span class="sxs-lookup"><span data-stu-id="60528-124">Exchange Server PowerShell (Exchange Management Shell)</span></span>](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)  
- [<span data-ttu-id="60528-125">Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="60528-125">Windows PowerShell</span></span>](http://msdn.microsoft.com/en-us/library/dd835506%28v=vs.85%29.aspx)
    

