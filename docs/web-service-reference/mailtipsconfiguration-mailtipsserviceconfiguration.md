---
title: MailTipsConfiguration (MailTipsServiceConfiguration)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsConfiguration
api_type:
- schema
ms.assetid: 9a34515e-815b-4c61-b118-d5f66b80238f
description: L’élément MailTipsConfiguration contient les informations de configuration de service pour le service de conseils de messagerie.
ms.openlocfilehash: 9128ee99545066899c3b27b624f10a9f1bd36c9d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: fr-FR
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467787"
---
# <a name="mailtipsconfiguration-mailtipsserviceconfiguration"></a><span data-ttu-id="4cf4d-103">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="4cf4d-103">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>

<span data-ttu-id="4cf4d-104">L’élément **MailTipsConfiguration** contient les informations de configuration de service pour le service de conseils de messagerie.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-104">The **MailTipsConfiguration** element contains service configuration information for the mail tips service.</span></span> 
  
```XML
<MailTipsConfiguration>
   <MailTipsEnabled/>
   <MaxRecipientsPerGetMailTipsRequest/>
   <MaxMessageSize/>
   <LargeAudienceThreshold/>
   <ShowExternalRecipientCount/>
   <InternalDomains/>
</MailTipsConfiguration>
```

 <span data-ttu-id="4cf4d-105">**MailTipsServiceConfiguration**</span><span class="sxs-lookup"><span data-stu-id="4cf4d-105">**MailTipsServiceConfiguration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4cf4d-106">Attributs et éléments</span><span class="sxs-lookup"><span data-stu-id="4cf4d-106">Attributes and elements</span></span>

<span data-ttu-id="4cf4d-107">Les sections suivantes décrivent les attributs, les éléments enfants et les éléments parents.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4cf4d-108">Attributs</span><span class="sxs-lookup"><span data-stu-id="4cf4d-108">Attributes</span></span>

<span data-ttu-id="4cf4d-109">Aucune.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4cf4d-110">Éléments enfants</span><span class="sxs-lookup"><span data-stu-id="4cf4d-110">Child elements</span></span>

|<span data-ttu-id="4cf4d-111">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4cf4d-111">**Element**</span></span>|<span data-ttu-id="4cf4d-112">**Description**</span><span class="sxs-lookup"><span data-stu-id="4cf4d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cf4d-113">MailTipsEnabled</span><span class="sxs-lookup"><span data-stu-id="4cf4d-113">MailTipsEnabled</span></span>](mailtipsenabled.md) <br/> |<span data-ttu-id="4cf4d-114">Indique si le service de conseils de messagerie est disponible.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-114">Indicates whether the mail tips service is available.</span></span> <span data-ttu-id="4cf4d-115">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="4cf4d-116">MaxRecipientsPerGetMailTipsRequest</span><span class="sxs-lookup"><span data-stu-id="4cf4d-116">MaxRecipientsPerGetMailTipsRequest</span></span>](maxrecipientspergetmailtipsrequest.md) <br/> |<span data-ttu-id="4cf4d-117">Indique le nombre maximal de destinataires pouvant être transmis à l' [opération GetMailTips](getmailtips-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4cf4d-117">Indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span> <span data-ttu-id="4cf4d-118">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-118">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="4cf4d-119">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="4cf4d-119">MaxMessageSize</span></span>](maxmessagesize.md) <br/> |<span data-ttu-id="4cf4d-120">Représente la taille maximale des messages qu’un destinataire peut accepter.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-120">Represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="4cf4d-121">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-121">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="4cf4d-122">LargeAudienceThreshold</span><span class="sxs-lookup"><span data-stu-id="4cf4d-122">LargeAudienceThreshold</span></span>](largeaudiencethreshold.md) <br/> |<span data-ttu-id="4cf4d-123">Représente le seuil d’audience élevée pour un client.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-123">Represents the large audience threshold for a client.</span></span> <span data-ttu-id="4cf4d-124">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-124">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="4cf4d-125">ShowExternalRecipientCount</span><span class="sxs-lookup"><span data-stu-id="4cf4d-125">ShowExternalRecipientCount</span></span>](showexternalrecipientcount.md) <br/> |<span data-ttu-id="4cf4d-126">Indique si les consommateurs de l' [opération GetMailTips](getmailtips-operation.md) doivent afficher des conseils de courrier qui indiquent le nombre de destinataires externes auxquels un message est adressé.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-126">Indicates whether consumers of the [GetMailTips operation](getmailtips-operation.md) have to show mail tips that indicate the number of external recipients to which a message is addressed.</span></span> <span data-ttu-id="4cf4d-127">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-127">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="4cf4d-128">InternalDomains (SmtpDomainList)</span><span class="sxs-lookup"><span data-stu-id="4cf4d-128">InternalDomains (SmtpDomainList)</span></span>](internaldomains-smtpdomainlist.md) <br/> |<span data-ttu-id="4cf4d-129">Identifie la liste des domaines SMTP internes de l’organisation.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-129">Identifies the list of internal SMTP domains of the organization.</span></span> <span data-ttu-id="4cf4d-130">Cet élément est obligatoire.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-130">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4cf4d-131">Éléments parents</span><span class="sxs-lookup"><span data-stu-id="4cf4d-131">Parent elements</span></span>

|<span data-ttu-id="4cf4d-132">**Élément**</span><span class="sxs-lookup"><span data-stu-id="4cf4d-132">**Element**</span></span>|<span data-ttu-id="4cf4d-133">**Description**</span><span class="sxs-lookup"><span data-stu-id="4cf4d-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cf4d-134">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="4cf4d-134">ServiceConfigurationResponseMessageType</span></span>](serviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="4cf4d-135">Contient les paramètres de configuration du service.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-135">Contains service configuration settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4cf4d-136">Valeur de texte</span><span class="sxs-lookup"><span data-stu-id="4cf4d-136">Text value</span></span>

<span data-ttu-id="4cf4d-137">Aucun.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-137">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4cf4d-138">Remarques</span><span class="sxs-lookup"><span data-stu-id="4cf4d-138">Remarks</span></span>

<span data-ttu-id="4cf4d-139">Le schéma qui décrit cet élément se trouve dans le répertoire virtuel IIS qui héberge les services web Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cf4d-139">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4cf4d-140">Informations sur l'élément</span><span class="sxs-lookup"><span data-stu-id="4cf4d-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4cf4d-141">Espace de noms</span><span class="sxs-lookup"><span data-stu-id="4cf4d-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4cf4d-142">Nom du schéma</span><span class="sxs-lookup"><span data-stu-id="4cf4d-142">Schema Name</span></span>  <br/> |<span data-ttu-id="4cf4d-143">Schéma Messages</span><span class="sxs-lookup"><span data-stu-id="4cf4d-143">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4cf4d-144">Fichier de validation</span><span class="sxs-lookup"><span data-stu-id="4cf4d-144">Validation File</span></span>  <br/> |<span data-ttu-id="4cf4d-145">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4cf4d-145">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4cf4d-146">Peut être vide</span><span class="sxs-lookup"><span data-stu-id="4cf4d-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="4cf4d-147">False</span><span class="sxs-lookup"><span data-stu-id="4cf4d-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4cf4d-148">Voir aussi</span><span class="sxs-lookup"><span data-stu-id="4cf4d-148">See also</span></span>



- [<span data-ttu-id="4cf4d-149">Éléments XML de EWS dans Exchange</span><span class="sxs-lookup"><span data-stu-id="4cf4d-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

