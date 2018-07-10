---
title: Référence de classe CChkSGFiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Trouvez des informations de référence pour l’API CHKSGFILES dans Exchange 2013.
ms.openlocfilehash: 583ac5e16ab60d119c3028bf81123e9f60a58ff4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19754747"
---
# <a name="cchksgfiles-class-reference"></a><span data-ttu-id="c252b-103">Référence de classe CChkSGFiles</span><span class="sxs-lookup"><span data-stu-id="c252b-103">CChkSGFiles class reference</span></span>

<span data-ttu-id="c252b-104">Trouvez des informations de référence pour l’API CHKSGFILES dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="c252b-104">Find reference information for the CHKSGFILES API in Exchange 2013.</span></span>
  
<span data-ttu-id="c252b-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="c252b-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="c252b-106">L’API CHKSGFILES permet aux applications de sauvegarde et de restauration vérifier l’intégrité des fichiers journaux des transactions Exchange Server 2013 et des bases de données par programme.</span><span class="sxs-lookup"><span data-stu-id="c252b-106">The CHKSGFILES API enables backup and restore applications to verify the integrity of Exchange Server 2013 transaction log files and databases programmatically.</span></span> <span data-ttu-id="c252b-107">Vous pouvez utiliser cette API de sauvegarde et restauration des applications qui utilisent le Volume Shadow Copy Service (VSS).</span><span class="sxs-lookup"><span data-stu-id="c252b-107">You can use this API in backup and restore applications that use the Volume Shadow Copy Service (VSS).</span></span>
  
> [!NOTE]
> <span data-ttu-id="c252b-108">Groupes de stockage ne sont pas disponibles dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="c252b-108">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="c252b-109">Prise en charge des groupes de stockage a été supprimé des versions d’Exchange commençant par Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="c252b-109">Support for storage groups was removed from versions of Exchange starting with Exchange Server 2010.</span></span> <span data-ttu-id="c252b-110">Pour assurer la compatibilité descendante avec les bases de données et les groupes de stockage dans les versions d’Exchange antérieures à Exchange 2010, l’API CHKSGFILES vous permet de spécifier les groupes de stockage.</span><span class="sxs-lookup"><span data-stu-id="c252b-110">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="c252b-111">Lorsque vous exécutez CHKSGFILES par rapport à des bases de données Exchange 2013, vous devez définir les paramètres que vous spécifiez un identificateur de groupe de stockage sur une chaîne vide.</span><span class="sxs-lookup"><span data-stu-id="c252b-111">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
## <a name="file-location"></a><span data-ttu-id="c252b-112">Emplacement de fichier</span><span class="sxs-lookup"><span data-stu-id="c252b-112">File location</span></span>
<span data-ttu-id="c252b-113"><a name="bk_fileslocation"> </a></span><span class="sxs-lookup"><span data-stu-id="c252b-113"></span></span>

<span data-ttu-id="c252b-114">L’API CHKSGFILES est fourni dans le cadre d’Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="c252b-114">The CHKSGFILES API ships as part of Exchange 2013.</span></span> <span data-ttu-id="c252b-115">Vous pouvez utiliser cette API sur un ordinateur ayant le rôle de serveur de boîtes aux lettres est installé.</span><span class="sxs-lookup"><span data-stu-id="c252b-115">You can use this API on a computer that has the Mailbox server role installed.</span></span> 
  
<span data-ttu-id="c252b-116">Par défaut, la DLL CHKSGFILES est installée dans le répertoire C:\Program Files\Microsoft\Exchange\V15\Bin.</span><span class="sxs-lookup"><span data-stu-id="c252b-116">By default, the CHKSGFILES DLL is installed in the C:\Program Files\Microsoft\Exchange\V15\Bin directory.</span></span>
  
<span data-ttu-id="c252b-117">Exchange 2013 inclut uniquement une version 64 bits (amd64) de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="c252b-117">Exchange 2013 includes only a 64-bit (amd64) version of the CHKSGFILES API.</span></span> 
  
<span data-ttu-id="c252b-118">Vous pouvez télécharger un fichier .zip qui inclut la bibliothèque CHKSGFILE.lib et fichiers d’en-tête CHKSGFILES.hxx pour une utilisation dans votre application personnalisée à partir du [Centre de téléchargement Microsoft](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="c252b-118">You can download a .zip file that includes the CHKSGFILE.lib library and CHKSGFILES.hxx header files for use in your custom application from the [Microsoft Download Center](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span></span>
  
## <a name="development-languages"></a><span data-ttu-id="c252b-119">Langages de développement</span><span class="sxs-lookup"><span data-stu-id="c252b-119">Development languages</span></span>
<span data-ttu-id="c252b-120"><a name="bk_developmentlanguages"> </a></span><span class="sxs-lookup"><span data-stu-id="c252b-120"></span></span>

<span data-ttu-id="c252b-121">L’API CHKSGFILES est destinée aux versions de Visual Studio commençant par Visual Studio 2005 dans C/C++ natif.</span><span class="sxs-lookup"><span data-stu-id="c252b-121">The CHKSGFILES API is intended for use with versions of Visual Studio starting with Visual Studio 2005 in native C/C++.</span></span> <span data-ttu-id="c252b-122">L’API CHKSGFILES n’est pas destiné à être utilisés dans du code managé.</span><span class="sxs-lookup"><span data-stu-id="c252b-122">The CHKSGFILES API is not intended for use in managed code.</span></span> <span data-ttu-id="c252b-123">Bien que vous pouvez créer un assembly d’interopérabilité COM avec CHKSGFILES, nous ne sont pas fournis un assembly d’interopérabilité COM pris en charge avec Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="c252b-123">Although you can create a COM Interop assembly with CHKSGFILES, we do not ship a supported COM Interop assembly with Exchange 2013.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="c252b-124">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="c252b-124">In this section</span></span>
<span data-ttu-id="c252b-125"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="c252b-125"></span></span>

- [<span data-ttu-id="c252b-126">Fonction CChkSGFiles.CMaxDbPerSG</span><span class="sxs-lookup"><span data-stu-id="c252b-126">CChkSGFiles.CMaxDbPerSG function</span></span>](cchksgfiles-cmaxdbpersg-function.md)
    
- [<span data-ttu-id="c252b-127">Fonction CChkSGFiles.Delete</span><span class="sxs-lookup"><span data-stu-id="c252b-127">CChkSGFiles.Delete function</span></span>](cchksgfiles-delete-function.md)
    
- [<span data-ttu-id="c252b-128">Énumération CChkSGFiles.ERR</span><span class="sxs-lookup"><span data-stu-id="c252b-128">CChkSGFiles.ERR enumeration</span></span>](cchksgfiles-err-enumeration.md)
    
- [<span data-ttu-id="c252b-129">Fonction CChkSGFiles.ErrCheckDbHeaders</span><span class="sxs-lookup"><span data-stu-id="c252b-129">CChkSGFiles.ErrCheckDbHeaders function</span></span>](cchksgfiles-errcheckdbheaders-function.md)
    
- [<span data-ttu-id="c252b-130">Fonction CChkSGFiles.ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="c252b-130">CChkSGFiles.ErrCheckDbPages function</span></span>](cchksgfiles-errcheckdbpages-function.md)
    
- [<span data-ttu-id="c252b-131">Fonction CChkSGFiles.ErrCheckLogs</span><span class="sxs-lookup"><span data-stu-id="c252b-131">CChkSGFiles.ErrCheckLogs function</span></span>](cchksgfiles-errchecklogs-function.md)
    
- [<span data-ttu-id="c252b-132">Fonction CChkSGFiles.ErrGetHeader (réservée)</span><span class="sxs-lookup"><span data-stu-id="c252b-132">CChkSGFiles.ErrGetHeader function (reserved)</span></span>](cchksgfiles-errgetheader-function-reserved.md)
    
- [<span data-ttu-id="c252b-133">Fonction CChkSGFiles.ErrInit</span><span class="sxs-lookup"><span data-stu-id="c252b-133">CChkSGFiles.ErrInit function</span></span>](cchksgfiles-errinit-function.md)
    
- [<span data-ttu-id="c252b-134">Fonction CChkSGFiles.ErrTerm</span><span class="sxs-lookup"><span data-stu-id="c252b-134">CChkSGFiles.ErrTerm function</span></span>](cchksgfiles-errterm-function.md)
    
- [<span data-ttu-id="c252b-135">Énumération CChkSGFiles.iDbInvalid</span><span class="sxs-lookup"><span data-stu-id="c252b-135">CChkSGFiles.iDbInvalid enumeration</span></span>](cchksgfiles-idbinvalid-enumeration.md)
    
- [<span data-ttu-id="c252b-136">Fonction CChkSGFiles.New</span><span class="sxs-lookup"><span data-stu-id="c252b-136">CChkSGFiles.New function</span></span>](cchksgfiles-new-function.md)
    
- [<span data-ttu-id="c252b-137">Énumération CChkSGFiles.NO_FLAGS</span><span class="sxs-lookup"><span data-stu-id="c252b-137">CChkSGFiles.NO_FLAGS enumeration</span></span>](cchksgfiles-no_flags-enumeration.md)
    
- [<span data-ttu-id="c252b-138">Struct CChkSGFiles.PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="c252b-138">CChkSGFiles.PAGE_INFO struct</span></span>](cchksgfiles-page_info-struct.md)
    
- [<span data-ttu-id="c252b-139">Fonction CChkSGFiles.PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="c252b-139">CChkSGFiles.PgnoFromFileOffset function</span></span>](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a><span data-ttu-id="c252b-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="c252b-140">See also</span></span>

- [<span data-ttu-id="c252b-141">Exchange Online et développement Exchange</span><span class="sxs-lookup"><span data-stu-id="c252b-141">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)
- [<span data-ttu-id="c252b-142">Sauvegarde, restauration et récupération d’urgence</span><span class="sxs-lookup"><span data-stu-id="c252b-142">Backup, Restore, and Disaster Recovery</span></span>](http://technet.microsoft.com/fr-fr/library/dd876874)
    

