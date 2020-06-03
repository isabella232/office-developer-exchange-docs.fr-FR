---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: L’élément ShowExternalRecipientCount indique si les consommateurs de l’opération GetMailTips doivent afficher des conseils de courrier électronique qui indiquent le nombre de destinataires externes auxquels un message est adressé.
ms.openlocfilehash: fc32e5c4a95f0e33b5532af9c77d31bd6446e641
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460469"
---
# <a name="showexternalrecipientcount"></a><span data-ttu-id="2d408-103">ShowExternalRecipientCount</span><span class="sxs-lookup"><span data-stu-id="2d408-103">ShowExternalRecipientCount</span></span>

<span data-ttu-id="2d408-104">L’élément **ShowExternalRecipientCount** indique si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) doivent afficher des conseils de courrier électronique qui indiquent le nombre de destinataires externes auxquels un message est adressé.</span><span class="sxs-lookup"><span data-stu-id="2d408-104">The **ShowExternalRecipientCount** element indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 <span data-ttu-id="2d408-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2d408-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d408-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="2d408-106">Attributes and elements</span></span>

<span data-ttu-id="2d408-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="2d408-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d408-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="2d408-108">Attributes</span></span>

<span data-ttu-id="2d408-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="2d408-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d408-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="2d408-110">Child elements</span></span>

<span data-ttu-id="2d408-111">Aucun.</span><span class="sxs-lookup"><span data-stu-id="2d408-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2d408-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="2d408-112">Parent elements</span></span>

|<span data-ttu-id="2d408-113">**Élément**</span><span class="sxs-lookup"><span data-stu-id="2d408-113">**Element**</span></span>|<span data-ttu-id="2d408-114">**Description**</span><span class="sxs-lookup"><span data-stu-id="2d408-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d408-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="2d408-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="2d408-116">Contient les informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="2d408-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2d408-117">Valeur texte</span><span class="sxs-lookup"><span data-stu-id="2d408-117">Text value</span></span>

<span data-ttu-id="2d408-118">La valeur texte de cet élément est **true** si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) doivent afficher des conseils de courrier électronique qui indiquent le nombre de destinataires externes auxquels un message est adressé.</span><span class="sxs-lookup"><span data-stu-id="2d408-118">The text value of this element is **true** if consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="2d408-119">La valeur est **false** si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) n’ont pas besoin d’afficher des conseils de courrier qui indiquent le nombre de destinataires externes auxquels un message est adressé.</span><span class="sxs-lookup"><span data-stu-id="2d408-119">The value is **false** if consumers of the [GetMailTips operation](getmailtips-operation.md) do not have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2d408-120">Remarques</span><span class="sxs-lookup"><span data-stu-id="2d408-120">Remarks</span></span>

<span data-ttu-id="2d408-121">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d408-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d408-122">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="2d408-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d408-123">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="2d408-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d408-124">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="2d408-124">Schema Name</span></span>  <br/> |<span data-ttu-id="2d408-125">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="2d408-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2d408-126">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="2d408-126">Validation File</span></span>  <br/> |<span data-ttu-id="2d408-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2d408-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d408-128">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="2d408-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="2d408-129">False</span><span class="sxs-lookup"><span data-stu-id="2d408-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d408-130">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="2d408-130">See also</span></span>



[<span data-ttu-id="2d408-131">Opération GetMailTips</span><span class="sxs-lookup"><span data-stu-id="2d408-131">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="2d408-132">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="2d408-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

