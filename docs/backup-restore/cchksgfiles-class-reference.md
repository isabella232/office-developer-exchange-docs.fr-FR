---
title: Référence de classe fonction cchksgfiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Recherchez des informations de référence pour l’API CHKSGFILES dans Exchange 2013.
ms.openlocfilehash: 38b1f2c900767c22594636f0c6ddf4855961aec4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526731"
---
# <a name="cchksgfiles-class-reference"></a><span data-ttu-id="ca441-103">Référence de classe fonction cchksgfiles</span><span class="sxs-lookup"><span data-stu-id="ca441-103">CChkSGFiles class reference</span></span>

<span data-ttu-id="ca441-104">Recherchez des informations de référence pour l’API CHKSGFILES dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ca441-104">Find reference information for the CHKSGFILES API in Exchange 2013.</span></span>
  
<span data-ttu-id="ca441-105">**S’applique à :** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="ca441-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="ca441-106">L’API CHKSGFILES permet aux applications de sauvegarde et de restauration de vérifier l’intégrité des fichiers journaux de transactions et des bases de données Exchange Server 2013 par programme.</span><span class="sxs-lookup"><span data-stu-id="ca441-106">The CHKSGFILES API enables backup and restore applications to verify the integrity of Exchange Server 2013 transaction log files and databases programmatically.</span></span> <span data-ttu-id="ca441-107">Vous pouvez utiliser cette API dans les applications de sauvegarde et de restauration qui utilisent le service VSS (Volume Shadow Copy Service).</span><span class="sxs-lookup"><span data-stu-id="ca441-107">You can use this API in backup and restore applications that use the Volume Shadow Copy Service (VSS).</span></span>
  
> [!NOTE]
> <span data-ttu-id="ca441-108">Les groupes de stockage ne sont pas disponibles dans Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ca441-108">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="ca441-109">La prise en charge des groupes de stockage a été supprimée des versions d’Exchange à partir d’Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="ca441-109">Support for storage groups was removed from versions of Exchange starting with Exchange Server 2010.</span></span> <span data-ttu-id="ca441-110">Pour assurer la compatibilité descendante avec les bases de données et les groupes de stockage dans les versions d’Exchange antérieures à Exchange 2010, l’API CHKSGFILES vous permet de spécifier des groupes de stockage.</span><span class="sxs-lookup"><span data-stu-id="ca441-110">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="ca441-111">Lorsque vous exécutez CHKSGFILES sur des bases de données Exchange 2013, vous devez définir des paramètres qui spécifient un identificateur de groupe de stockage sur une chaîne vide.</span><span class="sxs-lookup"><span data-stu-id="ca441-111">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
## <a name="file-location"></a><span data-ttu-id="ca441-112">Emplacement du fichier</span><span class="sxs-lookup"><span data-stu-id="ca441-112">File location</span></span>
<span data-ttu-id="ca441-113"><a name="bk_fileslocation"> </a></span><span class="sxs-lookup"><span data-stu-id="ca441-113"><a name="bk_fileslocation"> </a></span></span>

<span data-ttu-id="ca441-114">L’API CHKSGFILES est fournie dans le cadre d’Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ca441-114">The CHKSGFILES API ships as part of Exchange 2013.</span></span> <span data-ttu-id="ca441-115">Vous pouvez utiliser cette API sur un ordinateur sur lequel le rôle serveur de boîtes aux lettres est installé.</span><span class="sxs-lookup"><span data-stu-id="ca441-115">You can use this API on a computer that has the Mailbox server role installed.</span></span> 
  
<span data-ttu-id="ca441-116">Par défaut, la DLL CHKSGFILES est installée dans le répertoire C:\Program Files\Microsoft\Exchange\V15\Bin</span><span class="sxs-lookup"><span data-stu-id="ca441-116">By default, the CHKSGFILES DLL is installed in the C:\Program Files\Microsoft\Exchange\V15\Bin directory.</span></span>
  
<span data-ttu-id="ca441-117">Exchange 2013 inclut uniquement une version 64 bits (amd64) de l’API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="ca441-117">Exchange 2013 includes only a 64-bit (amd64) version of the CHKSGFILES API.</span></span> 
  
<span data-ttu-id="ca441-118">Vous pouvez télécharger un fichier. zip qui inclut la bibliothèque CHKSGFILE. lib et des fichiers d’en-tête CHKSGFILES. hxx à utiliser dans votre application personnalisée à partir du [Centre de téléchargement Microsoft](https://www.microsoft.com/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="ca441-118">You can download a .zip file that includes the CHKSGFILE.lib library and CHKSGFILES.hxx header files for use in your custom application from the [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=36802).</span></span>
  
## <a name="development-languages"></a><span data-ttu-id="ca441-119">Langages de développement</span><span class="sxs-lookup"><span data-stu-id="ca441-119">Development languages</span></span>
<span data-ttu-id="ca441-120"><a name="bk_developmentlanguages"> </a></span><span class="sxs-lookup"><span data-stu-id="ca441-120"><a name="bk_developmentlanguages"> </a></span></span>

<span data-ttu-id="ca441-121">L’API CHKSGFILES est conçue pour une utilisation avec les versions de Visual Studio à partir de Visual Studio 2005 en mode natif C/C++.</span><span class="sxs-lookup"><span data-stu-id="ca441-121">The CHKSGFILES API is intended for use with versions of Visual Studio starting with Visual Studio 2005 in native C/C++.</span></span> <span data-ttu-id="ca441-122">L’API CHKSGFILES n’est pas destinée à être utilisée dans du code managé.</span><span class="sxs-lookup"><span data-stu-id="ca441-122">The CHKSGFILES API is not intended for use in managed code.</span></span> <span data-ttu-id="ca441-123">Bien que vous puissiez créer un assembly d’interopérabilité COM avec CHKSGFILES, nous ne fournissons pas d’assembly d’interopérabilité COM pris en charge avec Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="ca441-123">Although you can create a COM Interop assembly with CHKSGFILES, we do not ship a supported COM Interop assembly with Exchange 2013.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="ca441-124">Dans cette section</span><span class="sxs-lookup"><span data-stu-id="ca441-124">In this section</span></span>
<span data-ttu-id="ca441-125"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="ca441-125"><a name="bk_inthissection"> </a></span></span>

- [<span data-ttu-id="ca441-126">Fonction fonction cchksgfiles. CMaxDbPerSG</span><span class="sxs-lookup"><span data-stu-id="ca441-126">CChkSGFiles.CMaxDbPerSG function</span></span>](cchksgfiles-cmaxdbpersg-function.md)
    
- [<span data-ttu-id="ca441-127">Fonction fonction cchksgfiles. Delete</span><span class="sxs-lookup"><span data-stu-id="ca441-127">CChkSGFiles.Delete function</span></span>](cchksgfiles-delete-function.md)
    
- [<span data-ttu-id="ca441-128">Fonction cchksgfiles. ERR, énumération</span><span class="sxs-lookup"><span data-stu-id="ca441-128">CChkSGFiles.ERR enumeration</span></span>](cchksgfiles-err-enumeration.md)
    
- [<span data-ttu-id="ca441-129">Fonction fonction cchksgfiles. ErrCheckDbHeaders</span><span class="sxs-lookup"><span data-stu-id="ca441-129">CChkSGFiles.ErrCheckDbHeaders function</span></span>](cchksgfiles-errcheckdbheaders-function.md)
    
- [<span data-ttu-id="ca441-130">Fonction fonction cchksgfiles. ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="ca441-130">CChkSGFiles.ErrCheckDbPages function</span></span>](cchksgfiles-errcheckdbpages-function.md)
    
- [<span data-ttu-id="ca441-131">Fonction fonction cchksgfiles. ErrCheckLogs</span><span class="sxs-lookup"><span data-stu-id="ca441-131">CChkSGFiles.ErrCheckLogs function</span></span>](cchksgfiles-errchecklogs-function.md)
    
- [<span data-ttu-id="ca441-132">Fonction fonction cchksgfiles. ErrGetHeader (réservée)</span><span class="sxs-lookup"><span data-stu-id="ca441-132">CChkSGFiles.ErrGetHeader function (reserved)</span></span>](cchksgfiles-errgetheader-function-reserved.md)
    
- [<span data-ttu-id="ca441-133">Fonction fonction cchksgfiles. ErrInit</span><span class="sxs-lookup"><span data-stu-id="ca441-133">CChkSGFiles.ErrInit function</span></span>](cchksgfiles-errinit-function.md)
    
- [<span data-ttu-id="ca441-134">Fonction fonction cchksgfiles. ErrTerm</span><span class="sxs-lookup"><span data-stu-id="ca441-134">CChkSGFiles.ErrTerm function</span></span>](cchksgfiles-errterm-function.md)
    
- [<span data-ttu-id="ca441-135">Fonction cchksgfiles. iDbInvalid, énumération</span><span class="sxs-lookup"><span data-stu-id="ca441-135">CChkSGFiles.iDbInvalid enumeration</span></span>](cchksgfiles-idbinvalid-enumeration.md)
    
- [<span data-ttu-id="ca441-136">Fonction fonction cchksgfiles. New</span><span class="sxs-lookup"><span data-stu-id="ca441-136">CChkSGFiles.New function</span></span>](cchksgfiles-new-function.md)
    
- [<span data-ttu-id="ca441-137">Fonction cchksgfiles. NO_FLAGS, énumération</span><span class="sxs-lookup"><span data-stu-id="ca441-137">CChkSGFiles.NO_FLAGS enumeration</span></span>](cchksgfiles-no_flags-enumeration.md)
    
- [<span data-ttu-id="ca441-138">Struct fonction cchksgfiles. PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="ca441-138">CChkSGFiles.PAGE_INFO struct</span></span>](cchksgfiles-page_info-struct.md)
    
- [<span data-ttu-id="ca441-139">Fonction fonction cchksgfiles. PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="ca441-139">CChkSGFiles.PgnoFromFileOffset function</span></span>](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a><span data-ttu-id="ca441-140">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="ca441-140">See also</span></span>

- [<span data-ttu-id="ca441-141">Développement d’Exchange et Exchange Online</span><span class="sxs-lookup"><span data-stu-id="ca441-141">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)
- [<span data-ttu-id="ca441-142">Sauvegarde, restauration et récupération d’urgence</span><span class="sxs-lookup"><span data-stu-id="ca441-142">Backup, Restore, and Disaster Recovery</span></span>](https://technet.microsoft.com/library/dd876874)
    

