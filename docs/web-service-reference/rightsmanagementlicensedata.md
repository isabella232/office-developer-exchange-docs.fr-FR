---
title: RightsManagementLicenseData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 38f0b7f4-2338-4e90-af67-e0951e8edfa3
description: L’élément RightsManagementLicenseData spécifie des informations sur la licence de gestion des droits pour un élément.
ms.openlocfilehash: ec2ba1dc155afe239c499246095f86fc621910a9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/25/2018
ms.locfileid: "19829234"
---
# <a name="rightsmanagementlicensedata"></a><span data-ttu-id="83687-103">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="83687-103">RightsManagementLicenseData</span></span>

<span data-ttu-id="83687-104">L’élément **RightsManagementLicenseData** spécifie des informations sur la licence de gestion des droits pour un élément.</span><span class="sxs-lookup"><span data-stu-id="83687-104">The **RightsManagementLicenseData** element specifies information about the rights management license for an item.</span></span> 
  
```XML
<RightsManagementLicenseData>
   <RightsManagedMessageDecryptionStatus/>
   <RmsTemplateId/>
   <TemplateName/>
   <TemplateDescription/>
   <EditAllowed/>
   <ReplyAllowed/>
   <ReplyAllAllowed/>
   <ForwardAllowed/>
   <ModifyRecipientsAllowed/>
   <ExtractAllowed/>
   <PrintAllowed/>
   <ExportAllowed/>
   <ProgrammaticAccessAllowed/>
   <IsOwner/>
   <ContentOwner/>
   <ContentExpiryDate/>
</RightsManagementLicenseData>
```

 <span data-ttu-id="83687-105">**RightsManagementLicenseDataType**</span><span class="sxs-lookup"><span data-stu-id="83687-105">**RightsManagementLicenseDataType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="83687-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="83687-106">Attributes and elements</span></span>

<span data-ttu-id="83687-107">Les sections suivantes décrivent les attributs, éléments enfants et éléments parents.</span><span class="sxs-lookup"><span data-stu-id="83687-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="83687-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="83687-108">Attributes</span></span>

<span data-ttu-id="83687-109">Aucun.</span><span class="sxs-lookup"><span data-stu-id="83687-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="83687-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="83687-110">Child elements</span></span>

<span data-ttu-id="83687-111">[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md) | [RMSTemplateId](rmstemplateid.md) | [TemplateName](templatename.md) | [TemplateDescription](templatedescription.md) | [EditAllowed](editallowed.md) | [ReplyAllowed](replyallowed.md)  |  [ ReplyAllAllowed](replyallallowed.md) | [ForwardAllowed](forwardallowed.md) | [ModifyRecipientsAllowed](modifyrecipientsallowed.md) | [ExtractAllowed](extractallowed.md) | [PrintAllowed](printallowed.md) | [ExportAllowed](exportallowed.md)  |  [ ProgrammaticAccessAllowed](programmaticaccessallowed.md) | [IsOwner](isowner.md) | [ContentOwner](contentowner.md) | [ContentExpiryDate](contentexpirydate.md)</span><span class="sxs-lookup"><span data-stu-id="83687-111">[RightsManagedMessageDecryptionStatus](rightsmanagedmessagedecryptionstatus.md) | [RMSTemplateId](rmstemplateid.md) | [TemplateName](templatename.md) | [TemplateDescription](templatedescription.md) | [EditAllowed](editallowed.md) | [ReplyAllowed](replyallowed.md) | [ReplyAllAllowed](replyallallowed.md) | [ForwardAllowed](forwardallowed.md) | [ModifyRecipientsAllowed](modifyrecipientsallowed.md) | [ExtractAllowed](extractallowed.md) | [PrintAllowed](printallowed.md) | [ExportAllowed](exportallowed.md) | [ProgrammaticAccessAllowed](programmaticaccessallowed.md) | [IsOwner](isowner.md) | [ContentOwner](contentowner.md) | [ContentExpiryDate](contentexpirydate.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="83687-112">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="83687-112">Parent elements</span></span>

<span data-ttu-id="83687-113">[Élément](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [tâche](task.md) | [PostItem ](postitem.md)  |  [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span><span class="sxs-lookup"><span data-stu-id="83687-113">[Item](item.md) | [Message](message-ex15websvcsotherref.md) | [MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [Task](task.md) | [PostItem](postitem.md) | [CalendarItem](calendaritem.md) | [Contact](contact.md) | [DistributionList](distributionlist.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="83687-114">Remarques</span><span class="sxs-lookup"><span data-stu-id="83687-114">Remarks</span></span>

<span data-ttu-id="83687-115">Cet élément est une nouveauté d'Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="83687-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="83687-116">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="83687-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="83687-117">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="83687-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="83687-118">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="83687-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="83687-119">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="83687-119">Schema name</span></span>  <br/> |<span data-ttu-id="83687-120">Schéma Types</span><span class="sxs-lookup"><span data-stu-id="83687-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="83687-121">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="83687-121">Validation file</span></span>  <br/> |<span data-ttu-id="83687-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="83687-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="83687-123">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="83687-123">Can be empty</span></span>  <br/> ||
   

